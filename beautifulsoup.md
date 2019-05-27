import requests
from bs4 import BeautifulSoup


url = "https://www.naver.com/"

response = requests.get(url).text
print(response)

soup = BeautifulSoup(response,'html.parser')

print(soup.prettify())