# Проект на тему: "Пешеходный Петербург"

## Применение в задачах культурологии: ##

1. Создать карту значимых объектов,
2. Классификация потребителей,
3. Построение маршрута,
4. Поиск кратчайшего пути от точки А до точки Б. 

### Как работать с библиотекой networkx? ###

Загружаем бибилиотеку:
```
{import networkx as nx}
```

Создаем пустой граф:
```
{graph = nx.Graph()}
```

Добавляем вершины в граф, используя метод add_node():
```
{graph.add_node('A')
graph.add_node('B')
graph.add_node('C')}
```

Создаем связи между объектами, соединяя вершины между собой, при помощи метода add_edge: 
```
{add_edge('A', 'B', graph=graph)
add_edge('B', 'C', graph=graph)}
```

Также мы можем указать расстояние между вершинами:
```
{graph.add_weighted_edges_from([("A", "B", 10),
                           ("B", "C", 15))]}
```

Наконец, визуализируем граф при помощи функции:
```
{nx.draw(graph, with_labels=True)}
```
ссылка на код: [тут] https://colab.research.google.com/drive/1RVPTesIBkfE_Ezd9AE__gIfFHoI-cgyk


## Применение библиотеки для решения нашей задачи: ##
1. Визуализация расстояния между наиболее значимыми достопримечательностями Петербурга в пеших прогулках.
2. Поиск кратчайшего пути от г.Чехов до г.Москва.

ссылка на код: [тут] https://colab.research.google.com/drive/1HdDvlMzFbS6w6YtEXIFv24clF_OnSpqK#scrollTo=7sNhJeGJRbPd


### Анализ результатов ###


### уровень 3 ###

~~зачеркнутыц текст

**жираный текст**

*курсив*

1. Применение в задачах культурологии: .....
2. Пример работы: (вставить код красиво)
3. Ссылка на код, мы применили библиотеку для нашей задачи.
4. Анализ результатов - выводы 


```
{python}
```

ссылка на код: [тут] https://colab.research.google.com/drive/1JM-4JgTAgceqUiQHPP4tPDbcoecYUFLD?usp=sharing

![здесь будет картинка](https://vtbrussia.ru/local/templates/picasso/css/images/share/picasso-share-cubism.jpg)
