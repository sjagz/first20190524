import random

# menu 리스트를 만들어주세요.

menu = ['20층','바스버거','양자강','백수산','시골집' ]

phonebook = {'20층': 1,'바스버거' : 2,'양자강' : 3,'백수산' : 4,'시골집' : 5}

choice = random.choice(menu)

phonebook[choice]

print(choice , phonebook[choice])