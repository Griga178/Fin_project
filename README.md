# Проект

## Описание

  распределение свечей по моментам, при наступлении определенный условий
  создание сигналов на открытие/закрытие позиции

  Возможности:
  - реализован "бот" осуществляющий торговлю через API на биржах Binance, Tinkoff
  - модуль анализа подбирающий коэффициенты для новых активов (настройка стратегии)
  - визуализация matplotlib.pyplot
  - сохранение отчетов в excel

## Визуализация
<ul>
<li><a href="#btcusdt-за-период-01012020-по-26102023">BTC/USDT 3 года (отчет, файл)</a></li>
<li><a href="#графики-1">BTC/USDT 3 года графики</a></li>
<li><a href="#графики-2">BTC/USDT 10 мес. графики</a></li>
<!-- <li><a href="#rasp-за-период-01012020-по-26102023">ОАО Распадская (RASP) 3 года (отчет, файл)</a></li> -->
</ul>

##  BTCUSDT за период 01.01.2020 по 26.10.2023

<a href = 'https://raw.githubusercontent.com/Griga178/Fin_project/master/files/BTCUSDT_2020.xlsx'> Ссылка на скачивание Excel файла(/files/BTCUSDT_2020.xlsx)</a>
<p> <i>в файле есть возможность поменять условия (реинвестирование/размер ставки/кредитное плечо)</i> </p>

<table>
  <thead>
    <th>Показатель</th>
    <th> Значение<br/>(лот = 1 у.е.)</th>
    <th> Значение<br/>(лот = 1 у.е. + пред. прибыль/убыток)</th>
  </thead>
  <tbody>
    <tr>
      <td align="left">Период</td>
      <td colspan="2" align="center">3 года 10 мес. (1392 дн.)</td>
    </tr>
    <tr>
      <td align="left">Чистая прибыль</td>
      <td colspan="1" align="center">375 %</td>
      <td colspan="1" align="center">1897 %</td>
    </tr>
    <tr>
      <td align="left">Чистая прибыль (в годовых)</td>
      <td colspan="1" align="center">98 %</td>
      <td colspan="1" align="center">116 %</td>
    </tr>
    <tr>
      <td align="left">Количество сделок всего</td>
      <td colspan="2" align="center">255</td>
    </tr>
    <tr>
      <td align="left">Количество положительных сделок</td>
      <td colspan="2" align="center">115</td>
    </tr>
    <tr>
      <td align="left">Сумма положительных сделок</td>
      <td colspan="1" align="center">7,81</td>
      <td colspan="1" align="center">38,10</td>
    </tr>
    <tr>
      <td align="left">Среднее положительных сделок</td>
      <td colspan="1" align="center">0,07</td>
      <td colspan="1" align="center">0,33</td>
    </tr>
    <tr>
      <td align="left">Вероятность наступления прибыльной сделки</td>
      <td colspan="2" align="center">0,469</td>
    </tr>
    <tr>
      <td align="left">Количество отрицательных сделок</td>
      <td colspan="2" align="center">130</td>
    </tr>
    <tr>
      <td align="left">Сумма отрицательных сделок</td>
      <td colspan="1" align="center">-4,05</td>
      <td colspan="1" align="center">-19,14</td>
    </tr>
    <tr>
      <td align="left">Среднее отрицательных сделок</td>
      <td colspan="1" align="center">-0,03</td>
      <td colspan="1" align="center">-0,15</td>
    </tr>
    <tr>
      <td align="left">Вероятность наступления отрицательной сделки</td>
      <td colspan="2" align="center">0,531</td>
    </tr>
    <tr>
      <td align="left">Отношение кол-ва прибыльных сделок к убыточным</td>
      <td colspan="2" align="center">0,88</td>
    </tr>
    <tr>
      <td align="left">Профит-фактор</td>
      <td colspan="1" align="center">2,176</td>
      <td colspan="1" align="center">2,251</td>
    </tr>
    <tr>
      <td align="left">Математическое ожидание 1</td>
      <td colspan="1" align="center">0,02</td>
      <td colspan="1" align="center">0,08</td>
    </tr>
    <tr>
      <td align="left">Математическое ожидание 2</td>
      <td colspan="1" align="center">2,93</td>
      <td colspan="1" align="center">2,99</td>
    </tr>    
    <tr>
      <td align="left">Максимальная просадка</td>
      <td colspan="1" align="center">15 %</td>
      <td colspan="1" align="center">29 %</td>
    </tr>  
    <tr>
      <td align="left">Фактор восстановления</td>
      <td colspan="1" align="center">24,86</td>
      <td colspan="1" align="center">64,89</td>
    </tr>
  </tbody>
</table>

<p>Математическое ожидание 1: </br>"сумма положительный сделок" * "кол-во положительный сделок" / "сумма отрицательных сделок" * "кол-во отрицательных сделок"</p>
<p>Математическое ожидание 2: </br>1 + "кол-во положительный сделок" / "кол-во отрицательных сделок" * "Профит-фактор"</p>
<p>Профит-фактор: </br>
"Среднее положительных сделок" / "Среднее отрицательных сделок" * (-1)</p>

## Графики 1
### Результаты сделок: ("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_1.png)
### Результаты сделок: Сумма("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_2.png)
### Сигналы на графике
  ![plot](/plots/Figure_3.png)

## Графики 2
## период 01.01.2023 по 26.10.2023
### Результаты сделок ("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_1_2.png)
### Результаты сделок Сумма("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_2_2.png)
### Сигналы на графике
  ![plot](/plots/Figure_3_2.png)
<!--
## RASP за период 01.01.2020 по 26.10.2023
<a href = 'https://raw.githubusercontent.com/Griga178/Fin_project/master/files/RASPRUB_2020.xlsx'> Ссылка на скачивание Excel файла(/files/RASPRUB_2020.xlsx)</a>
<p> <i>в файле есть возможность поменять условия (реинвестирование/размер ставки/кредитное плечо)</i> </p>

  <table>
    <thead>
      <th>Показатель</th>
      <th> Значение<br/>(лот = 1 у.е.)</th>
      <th> Значение<br/>(лот = 1 у.е. + пред. прибыль/убыток)</th>
    </thead>
    <tbody>
      <tr>
        <td align="left">Период</td>
        <td colspan="2" align="center">3 года 10 мес. (1392 дн.)</td>
      </tr>
      <tr>
        <td align="left">Чистая прибыль</td>
        <td colspan="1" align="center">187 %</td>
        <td colspan="1" align="center">456 %</td>
      </tr>
      <tr>
        <td align="left">Чистая прибыль (в годовых)</td>
        <td colspan="1" align="center">49,03 %</td>
        <td colspan="1" align="center">49 %</td>
      </tr>
      <tr>
        <td align="left">Количество сделок всего</td>
        <td colspan="2" align="center">105</td>
      </tr>

      <tr>
        <td align="left">Количество положительных сделок</td>
        <td colspan="2" align="center">55</td>
      </tr>
      <tr>
        <td align="left">Сумма положительных сделок</td>
        <td colspan="1" align="center">3,02</td>
        <td colspan="1" align="center">7,23</td>
      </tr>
      <tr>
        <td align="left">Среднее положительных сделок</td>
        <td colspan="1" align="center">0,05</td>
        <td colspan="1" align="center">0,13</td>
      </tr>
      <tr>
        <td align="left">Вероятность наступления прибыльной сделки</td>
        <td colspan="2" align="center">0,524</td>
      </tr>
      <tr>
        <td align="left">Количество отрицательных сделок</td>
        <td colspan="2" align="center">50</td>
      </tr>
      <tr>
        <td align="left">Сумма отрицательных сделок</td>
        <td colspan="1" align="center">-1,15</td>
        <td colspan="1" align="center">-2,67</td>
      </tr>
      <tr>
        <td align="left">Среднее отрицательных сделок</td>
        <td colspan="1" align="center">-0,02</td>
        <td colspan="1" align="center">-0,05</td>
      </tr>
      <tr>
        <td align="left">Вероятность наступления отрицательной сделки</td>
        <td colspan="2" align="center">0,476</td>
      </tr>
      <tr>
        <td align="left">Отношение кол-ва прибыльных сделок к убыточным</td>
        <td colspan="2" align="center">1,1</td>
      </tr>
      <tr>
        <td align="left">Профит-фактор</td>
        <td colspan="1" align="center">2,46</td>
        <td colspan="1" align="center">2,38</td>
      </tr>
      <tr>
        <td align="left">Математическое ожидание 1</td>
        <td colspan="1" align="center">0,02</td>
        <td colspan="1" align="center">0,04</td>
      </tr>
      <tr>
        <td align="left">Математическое ожидание 2</td>
        <td colspan="1" align="center">3,62</td>
        <td colspan="1" align="center">3,71</td>
      </tr>    
      <tr>
        <td align="left">Максимальная просадка</td>
        <td colspan="1" align="center">15 %</td>
        <td colspan="1" align="center">16 %</td>
      </tr>  
      <tr>
        <td align="left">Фактор восстановления</td>
        <td colspan="1" align="center">12,51</td>
        <td colspan="1" align="center">29,32</td>
      </tr>
    </tbody>
  </table>

Математическое ожидание 1: "сумма положительный сделок" * "кол-во положительный сделок" / "сумма отрицательных сделок" * "кол-во отрицательных сделок"
Математическое ожидание 2: 1 + "кол-во положительный сделок" / "кол-во отрицательных сделок" * "Профит-фактор" -->


Опираясь на реализованную стратегию веду торговлю с июня 2023 года на Binance и Tinkoff, до этого периодически торговал, не имея четкой стратегии с 2016г.
