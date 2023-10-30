# Проект

## Описание

  распределение свечей по моментам, при наступлении определенный условий
  создание сигналов на открытие/закрытие позиции

  - реализован "бот" осуществляющий торговлю через API на биржах Binance, Tinkoff
  - модуль анализа подбирающий коэффициенты для новых активов (настройка стратегии)
  - визуализация matplotlib.pyplot
  - сохранение отчетов в excel

## Визуализация
<ul>
<li><a href="#btcusdt-за-период-01012020-по-26102023">BTC/USDT 3 года отчет, файл</a></li>
<li><a href="#графики-1">BTC/USDT 3 года графики</a></li>
<li><a href="#графики-2">BTC/USDT 10 мес. графики</a></li>
<li><a href="#rasp-за-период-01012020-по-26102023">ОАО Распадская (RASP)3 года</a></li>
</ul>

##  BTCUSDT за период 01.01.2020 по 26.10.2023

<a href = 'https://raw.githubusercontent.com/Griga178/Fin_project/master/files/BTCUSDT_2020.xlsx'> Ссылка на скачивание Excel файла(/files/BTCUSDT_2020.xlsx)</a>
<p> <i>в файле есть возможность поменять условия</i> </p>

<table>
  <thead>
    <th>Показатель</th>
    <th> Значение<br/>(лот = 1 у.е.)</th>
    <th> Значение<br/>(лот = предыдущий результат)</th>
  </thead>
  <tbody>
    <tr>
      <td align="left">Количество сделок</td>
      <td colspan="2" align="center">255</td>
    </tr>
    <tr>
      <td align="left">Сумма сделок (Прибыль)</td>
      <td colspan="1" align="center">3,75</td>
      <td colspan="1" align="center">18,97</td>
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
      <td align="left">Отношение кол-ва прибыльных сделок к убыточным</td>
      <td colspan="2" align="center">0,88</td>
    </tr>
    <tr>
      <td align="left">Профит-фактор</td>
      <td colspan="1" align="center">2,176</td>
      <td colspan="1" align="center">2,251</td>
    </tr>
    <tr>
      <td align="left">Вероятность наступления прибыльной сделки</td>
      <td colspan="2" align="center">0,469</td>
    </tr>
    <tr>
      <td align="left">Вероятность наступления отрицательной сделки</td>
      <td colspan="2" align="center">0,531</td>
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

  </tbody>
</table>

## Графики 1
### Результаты сделок ("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_1.png)
### Результаты сделок Сумма("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_2.png)
### Сигналы на графике
  ![plot](/plots/Figure_3.png)

## Графики 2
## период 01.01.2020 по 26.10.2023
### Результаты сделок ("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_1_2.png)
### Результаты сделок Сумма("Цена покупки" / "Цена продажи" - 1)
  ![plot](/plots/Figure_2_2.png)
### Сигналы на графике
  ![plot](/plots/Figure_3_2.png)

## RASP за период 01.01.2020 по 26.10.2023

  Результаты применения стратегии на исторических данных за 3 года (с 02.08.2020), прибыль - реинвестируется, кредитное плечо - отсутствует:

  BTC / USDT
  Количество сделок: 204 шт.
  Отношение кол-ва прибыльных сделок к убыточным: 0,91 (97/107)
  Прибыль за 3 года: 998,9% (+1883,73%, -884,83%)
  Средняя прибыль в год: 115%
  Максимальная просадка: 29%
  Профит фактор: 2,35 (19,42/8,27)
  Фактор восстановления: 34,18
  Мат. ожидание*: 3,13
  (без реинвестирования, прибыль за 3 года: 278%, просадка: 18%)

  *Мат. ожидание = 1 + "Профит фактор" * "Отношение кол-ва прибыльных сделок к убыточным".

Опираясь на реализованную стратегию веду торговлю с июня 2023 года на Binance и Tinkoff, до этого периодически торговал, не имея четкой стратегии с 2016г.
