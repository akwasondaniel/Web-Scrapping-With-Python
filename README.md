# Web-Scrapping-With-Python

<--! Importing Beautifulsoup libary and request to enable me pull data from jiji.com html website>

from bs4 import BeautifulSoup
import requests

<--! 

list of data to scrap from jiji
name
brand
price
location
ram
internal_storage
color
condition
>


<--! defining my parameters >
html_text = requests.get('https://jiji.ng/mobile-phones').text
soup = BeautifulSoup(html_text, 'lxml')
print(html_text)
