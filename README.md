# Проект на тему: "Graph Peter"

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

Наконец, визуализируем граф:
```
{nx.draw(graph, with_labels=True)}
```
![здесь будет картинка](https://github.com/Blazheska/project_Blazheska/blob/main/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.png?raw=true)



ссылка на код: [тут] https://colab.research.google.com/drive/1RVPTesIBkfE_Ezd9AE__gIfFHoI-cgyk


## Применение библиотеки для решения нашей задачи: ##
1. Визуализация расстояния между наиболее значимыми достопримечательностями Петербурга в пеших прогулках.
2. Поиск кратчайшего пути от г.Чехов до г.Москва.

![здесь будет картинка](https://github.com/Blazheska/project_Blazheska/blob/main/%D0%9D%D0%BE%D0%BC%D0%B5%D1%80%201.png?raw=true)

ссылка на код: [тут] https://colab.research.google.com/drive/1HdDvlMzFbS6w6YtEXIFv24clF_OnSpqK#scrollTo=7sNhJeGJRbPd

### Анализ результатов ###

В результате проделанной работы при помощи библиотеки networkx была создана визуальная схема пешей прогулки по Петербургу. 
На графике вида digraph показаны наиболее короткие расстояния между объектами. 
