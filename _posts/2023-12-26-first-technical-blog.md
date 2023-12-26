---
title: "first-technical-blog"
date: 2023-12-26
---
# Python Lists and Dictionaries

## Lists

- double veya single quote ayni

```
print("Pluto's a planet!")
print('My dog is named "Pluto"')
```

- araya single quote koymak icin backspace / kulan`'Pluto**\'**s a planet!'`
- uclu quote kullaninca yeni satir otomatik olusturur

```
triplequoted_hello = """hello
world"""
```

- `print("hello", end='')`   print sonuna end koyarsan yeni satira atlamaz.
- String lerde sequence gibidir. MyString[0] diye karakterlere ulasabilirsin ancak immutable dirler, yani degistiremezsin
- claim bir string ise —>  claim.upper()         claim.lower         claim.index(’plan’)       methodlari kullanilabilir
- string.split()   string’i list’e donderir, bosluklar ayirici default olarak
- string.join()    bircok stringi bir tane uzun stringe birlestirir
- `'/'.join([month, day, year])`        output: `'01/31/1956'`
- Stringleri concatenate etmek icin + kullanilabilir  `planet + ', we miss you.'`           Output: `'Pluto, we miss you.'`
- Ancak boyle yaparken araya string olmayan birsey koymak istersek, onu str() kullanarak stringe cevirmeliyiz

```
#bu kod hata verir cunku 9 arada string degil
position = 9
planet + ", you'll always be the " + position + "th planet to me."      # WRONG
planet + ", you'll always be the " + str(position) + "th planet to me."   #CORRECT
```

- Dogru ama okumasi zor olmaya basladi o yuzden .format() kullanmak epey okunurlulugu arttiriyor.

`"**{}**, you'll always be the **{}**th planet to me.".format(planet, position)`

Burada {} placeholders. Bu format daha iyi

**You could probably write a short book just on `str.format`, so I'll stop here, and point you to [pyformat.info](https://pyformat.info/) and [the official docs](https://docs.python.org/3/library/string.html#formatstrings) for further reading.**

## Dictionaries

Dictionaries are a built-in Python data structure for mapping keys to values.

`numbers = {'one':1, 'two':2, 'three':3}`

`numbers['eleven'] = 11`  #to add new key-value pair

e can access a collection of all the keys or all the values with `dict.keys()` and `dict.values()`, respectively.

[Kutuphaneler](https://www.notion.so/Kutuphaneler-1c8b3d733bb54d9a818123f1df0a81bd?pvs=21)

[****External Libraries****](https://www.notion.so/External-Libraries-f4a040857389437db3ffae677377275b?pvs=21)

## General Python Problems (Basic)

round()   →nearest integere yuvarlar

int()   →bir alt integere yuvarlar
