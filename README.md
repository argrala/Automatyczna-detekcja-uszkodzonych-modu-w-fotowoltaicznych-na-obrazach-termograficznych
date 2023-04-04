# Projekt detekcji defektów modułów fotowoltaicznych
Celem było stworzenie modułu detekcyjnego, który mogłby zostać wykorzystany do systemu automatycznej detekcji uszkodzeń w modułach fotowoltaicznych. 
Celem projektu było zbadanie przydatności głębokich sieci neuronowych w zagadnieniu detekcji uszkodzeń modułów fotowoltaicznych oraz porównanie działania różnych modeli konwolucyjnych sieci neuronowych, w kontekście zdjęć termograficznych modułów solarnych. Kluczowe było również opracowanie modelu detekcyjnego, który mógłby stanowić element automatycznego systemu diagnostycznego.

![Zrzut ekranu z 2022-10-31 04-34-42](https://user-images.githubusercontent.com/98141690/229655358-1fcf72ac-53fc-4943-bb38-74f7c1c44a29.png)

Przykładowy system składający się z bezzałogowego statku powietrznego, kamery termograficznej, zaprogramowanej trasy lotu i detektora defektów.

# Motywacja
Rosnący popyt na energię słoneczną przyczynia się do dynamicznego wzrostu powierzchni przeznaczanej na elektrownie słoneczne. W związku z tym powstaje potrzeba opracowania efektywnych metod diagnostycznych. Automatyczny system detekcji uszkodzeń w modułach fotowoltaicznych pozwoli na szybką i skuteczną identyfikację defektów.

# Zbiór danych
Modele zostały wyuczone przy wykorzystaniu niepublicznego zbioru danych zawierającego zdjęcia termowizyjne farm fotowoltaicznych z oznaczonymi zklasyfikowanymi modułami słonecznymi w formacie Pascal VOC.

![obraz](https://user-images.githubusercontent.com/98141690/229657837-69bc0fc3-df3a-48a4-8bec-2ba7e3db77f7.png)

Przykładowe defekty modułów fotowoltaicznych

Modele YOLOv5_obb, S2A-net i Oriented-rcnn wykorzystują format anotacji DOTA, natomiast YOLOv7 używa formatu YOLO.
# Wykorzystane narzędzia
Najważniejszym wykorzystanym narzędziem była platforma Colaboratory od Google Research, która zapewniła zdalny dostęp do wydajnych kart. Kluczowe były projekty MMRotate, YOLOv7 oraz YOLOv5_obb dzięki którym wyuczono i obsługiwano detektory. Przydatne do obróbki i testów zbioru danych okazały się narzędzia roboflow i MakeSense.
![obraz](https://user-images.githubusercontent.com/98141690/229656168-ed303b5d-2c71-41d2-83aa-7331c5e9e6dd.png)

# Podsumowanie
Projekt zakończył się powodzeniem, udało się wyuczyć dwa modele, które nadają się do zastosowania jako detektor w systemie automatycznego nadzoru. Osiągnięto bardzo dobre wyniki dla modeli YOLOv7 i Oriented R-CNN. Wykazano użyteczność głębokich sieci neuronowych w zagadnieniu detekcji uszkodzeń modułów fotowoltaicznych.
![obraz](https://user-images.githubusercontent.com/98141690/229655852-84c3518f-1928-48ae-a8b8-8246931c7f94.png)
