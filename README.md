# common_lit


Report

### Какую решаем задачу?

* Оценить сложность текста для чтения (Градация 3-12 класс)

### Требование к модели:

#### Функциональные
* Модель должна учитывать свзяность и семантику текста

#### Не функциональные
* CPU <= 3 часа работы
* GPU <= 3 часа работы

### Метрика 
* RMSE

### Data

Base

id - unique ID for excerpt
url_legal - URL of source - this is blank in the test set.
license - license of source material - this is blank in the test set.
excerpt - text to predict reading ease of
target - reading ease
standard_error - measure of spread of scores among multiple raters for each excerpt. Not included for test data.


### Существующие методы:

* Flesch-Kincaid Grade Level are based on weak proxies of text decoding (characters or syllables per word) 
and syntactic complexity (i.e., number or words per sentence). As a result, they lack construct and theoretical validity. 

* At the same time, commercially available formulas, such as Lexile, 
can be cost-prohibitive, lack suitable validation studies, 
and suffer from transparency issues when the formula's features aren't publicly available.
