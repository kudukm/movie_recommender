# Movie recommender
Niniejszy model na podstawie ocen filmów przedstawionych przez użytkownika zwraca 5 proponowanych filmów, które podobały się innym o podobnych preferencjach.

## Katalog data/
Zawiera dane, na których uczony był model z [MovieLens Dataset](https://grouplens.org/datasets/movielens/).

## main.ipynb
Zawiera działajacy model.
### class DataLoader
Wczytuje dane z plików.
### class DataPreprocessor
Przekształca dane wejściowe na potrzeby modelu
### class RecommenderModel
Przewiduje oceny filmów.
### def recommend_movies_from_terminal()
Pozwala użytkownikowi ocenić wybrane filmy i na ich podstawie zwraca takie, które podobały się innym widzom o podobnych preferencjach.

## Przykład użycia
### Wejście:
W pierwszym okienku podajemy oddzielone przecinkami nazwy filmów, a w drugim w tej samej kolejności ich oceny.
```
movies_list = ["Toy Story", "Avengers", "The Iron Giant"]  
ratings_list = [4, 5, 3]
```
### Wyjście:
```
Recommendations:  
Wings of Courage  
Blue in the Face  
Kids  
Immortal Beloved  
Surviving the Game
```

## Wymagania
* Menadżer pakietów Conda z zainstalowanym Jupyter Notebook
* Biblioteki Pythona:
    * joblib 1.4.2
    * numpy 1.26.4
    * pandas 2.2.2
    * python-dateutil 2.9.0.post0
    * pytz 2024.1
    * scikit-learn 1.5.0
    * scipy 1.13.1
    * six 1.16.0
    * threadpoolctl  3.5.0
    * tzdata 2024.1
