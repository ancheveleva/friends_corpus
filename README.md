#   FRIENDS CORPUS

Привет! Это протоверсия корпуса по сериалу «Друзья».

## 0. Начало работы
Чтобы воспользоваться поиском, тебе нужно:
1. Cкачать [Базу Данных](https://drive.google.com/drive/folders/1D6TELFeLOES34owP4dX51dsmi9YT-fJu?usp=sharing)
2. Cкачать из этого репозитория тетрадку [2_search.ipynb](https://github.com/ancheveleva/friends_corpus/blob/main/2_search.ipynb)
3. Положить тетрадку и БД в одну директорию и запустить её в jupyter notebook или Google Colab
4. Готово! Теперь ты можешь искать всякое? Какое всякое? См. п.1!


## 1. Правила поиска
Поиск доступен в трёх форматах:
- по точному словоупотреблению: слово в кавычках, одинарных или двойных (не ёлочки!)
- по лемме: слово без ковычек
- по лемме+ЧР_тег (частеречный тег см. п.3): слово_без_кавычек+ЧР_тег 

Максимальная длина запроса: 3, форматы можно комбинировать

Примеры запросов:
- how AUX you do
- how be you "doing"
- what do+AUX you do+VERB


## 2. Выдача результатов
Результаты сохраняются в файл results.csv

**Внимание!** При каждом запросе файл обновляется. Если тебе нужно сохранить результаты нескольких запросов, переименовывай файн reɬusts.csv после его формирования.


## 3. Набор тегов
Данный корпус использует для разметки анализатор spaCy, который в свою очередь использует [Universal POS tags](https://universaldependencies.org/u/pos/)

|Open class words|Closed class words|Other|
|---|---|---|		
|ADJ|ADP|PUNCT|
|ADV|AUX|SYM|
|INTJ|CCONJ|X|
|NOUN|DET||
|PROPN|NUM||	 
|VERB|PART|| 
||PRON|| 
||SCONJ||

Расшифровка тегов:
- ADJ: adjective
- ADP: adposition
- ADV: adverb
- AUX: auxiliary
- CCONJ: coordinating conjunction
- DET: determiner
- INTJ: interjection
- NOUN: noun
- NUM: numeral
- PART: particle
- PRON: pronoun
- PROPN: proper noun
- PUNCT: punctuation
- SCONJ: subordinating conjunction
- SYM: symbol
- VERB: verb
- X: other
