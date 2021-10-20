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
graph.add_node('C')
graph.add_node('D')}
```

Создаем связи между объектами, соединяя вершины между собой, при помощи метода add_edge: 
```
{add_edge('A', 'B', graph=graph)
add_edge('B', 'C', graph=graph)
add_edge('C', 'D', graph=graph)}
```

Также мы можем указать расстояние между вершинами:
```
{graph.add_weighted_edges_from([("A", "B", 10),
                                ("B", "C", 15),
                                ("C", "D", 15),
                                ("A", "D", 5),
                                ("B", "D", 3)])
```

Наконец, визуализируем граф:
```
{nx.draw(graph, with_labels=True)}
```

![здесь будет картинка](https://github.com/Blazheska/project_Blazheska/blob/main/%D0%9D%D0%BE%D0%BC%D0%B5%D1%80%203.png?raw=true)

ссылка на код: [тут] https://colab.research.google.com/drive/1RVPTesIBkfE_Ezd9AE__gIfFHoI-cgyk


Зная расстояние между вершинами, мы можем найти кратчайший путь от точки А до точки B.

![здесь будет картинка](https://github.com/Blazheska/project_Blazheska/blob/main/%D0%9D%D0%BE%D0%BC%D0%B5%D1%80%202.png?raw=true) 

ссылка на код: [тут] https://colab.research.google.com/drive/1HdDvlMzFbS6w6YtEXIFv24clF_OnSpqK#scrollTo=7sNhJeGJRbPd


### Примеры создания пустых графов различного типа ###

```
{G=nx.Graph()}
```
```
{G=nx.DiGraph()}
```
```
{G=nx.MultiGraph()}
```
```
{G=nx.MultiDiGraph()}
```


## Применение библиотеки для решения нашей задачи: ##
1. Визуализация расстояния между наиболее значимыми достопримечательностями Петербурга в пеших прогулках.
2. Поиск кратчайшего пути от г.Чехов до г.Москва.

![здесь будет картинка](https://github.com/Blazheska/project_Blazheska/blob/main/%D0%9D%D0%BE%D0%BC%D0%B5%D1%80%201.png?raw=true)

ссылка на код: [тут] https://colab.research.google.com/drive/1HdDvlMzFbS6w6YtEXIFv24clF_OnSpqK#scrollTo=7sNhJeGJRbPd

### Анализ результатов ###

В результате проделанной работы при помощи библиотеки networkx была создана визуальная схема пешей прогулки по Петербургу. 
На графике вида digraph показаны наиболее короткие расстояния между объектами. 
