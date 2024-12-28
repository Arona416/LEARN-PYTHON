### A.Классная точка
```
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y   
```
### B.Классная точка 2.0
```
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def move(self, shift_x, shift_y):
        self.x += shift_x
        self.y += shift_y

    def length(self, p):
        return round(((self.x - p.x)**2 + (self.y - p.y)**2)**0.5, 2)
```
### C.Не нажимай красную кнопку!
```
class RedButton:
    def __init__(self):
        self.counter = 0

    def click(self):
        print('Тревога!')
        self.counter += 1

    def count(self):
        return self.counter
```
### D.Работа не волк
```
class Programmer:

    def __init__(self, name, position="Junior"):
        self.name = name
        self.position = position
        self.worked = 0
        self.money = 0
        self.overrises = 0

    def work(self, time):
        P = {
            "Junior": 10,
            "Middle": 15,
            "Senior": 20,
        }
        self.worked += time
        self.money += time * (P[self.position] + self.overrises)

    def rise(self):
        if self.position == "Junior":
            self.position = "Middle"
        elif self.position == "Middle":
            self.position = "Senior"
        elif self.position == "Senior":
            self.overrises += 1

    def info(self):
        return f'{self.name} {self.worked}ч. {self.money}тгр.'
```
### E.Классный прямоугольник
```
class Rectangle:
    def __init__(self, *coords):
        self.coords = coords
        self.first_line = abs(self.coords[0][0] - self.coords[1][0])
        self.second_line = abs(self.coords[0][1] - self.coords[1][1])

    def perimeter(self):
        return round(2 * (self.first_line + self.second_line), 2)

    def area(self):
        return round(self.first_line * self.second_line, 2)
```
### F.Классный прямоугольник 2.0
```
class Rectangle:
    def __init__(self, *coords):
        self.coords = coords
        self.upper_left_x = round(min(self.coords[0][0], self.coords[1][0]), 2)
        self.upper_left_y = round(max(self.coords[0][1], self.coords[1][1]), 2)
        self.lower_right_x = round(max(self.coords[0][0], self.coords[1][0]), 2)
        self.lower_right_y = round(min(self.coords[0][1], self.coords[1][1]), 2)
        self.width = abs(self.coords[0][0] - self.coords[1][0])
        self.height = abs(self.coords[0][1] - self.coords[1][1])

    def perimeter(self):
        return round(2 * (self.width + self.height), 2)

    def area(self):
        return round(self.width * self.height, 2)

    def get_pos(self):
        return self.upper_left_x, self.upper_left_y

    def get_size(self):
        return round(self.width, 2), round(self.height, 2)

    def move(self, dx, dy):
        self.coords = (self.coords[0][0] + dx, self.coords[0][1] + dy), (self.coords[1][0] + dx, self.coords[1][1] + dy)
        self.__init__(*self.coords)

    def resize(self, width, height):
        self.coords = self.get_pos(), (self.upper_left_x + width, self.upper_left_y - height)
        self.__init__(*self.coords)
```
