# Yandex handbook "Python Basics" answers

## 2.1. Ввод и вывод данных. Операции с числами, строками. Форматирование

### A. Привет, Яндекс!
```
print("Привет, Яндекс!")
```

### B.Привет, всем!
```
username = input("Как Вас зовут?")
print(f"Привет, {username}")
```
### C.Излишняя автоматизация
```
formule = input()
print(f"{formule} \n" * 3)
```
### D.Сдача
```
money = int(input())
price = 2.5 * 38 
print(int(money - price))
```
### E.Магазин
```
prix_produit = int(input())
poids_mar = int(input())
my_money = int(input())
prix_tot = prix_produit * poids_mar
print(my_money - prix_tot)
```
### F.Чек
```
name_pro = input()  # Nom du produit
price = int(input())  # Prix par kg
poids = int(input())  # Poids en kg
som_tot = price * poids  # Somme totale

my_money = int(input())  # Argent donné
rest = my_money - som_tot  # Monnaie à rendre

# Affichage du reçu avec le bon format
print("Чек")
print(f"{name_pro} - {poids}кг - {price}руб/кг")
print(f"Итого: {som_tot}руб")
print(f"Внесено: {my_money}руб")
print(f"Сдача: {rest}руб")
```
### G.Делу — время, потехе — час
```
phrase = str("Купи слона!")
repet_nb = int(input())
print((phrase + "\n") * repet_nb)
```
### H.Наказание
```
nomber_rep = int(input())  # Nombre de répétitions
phrase = input()  # Phrase à répéter

# Création de la chaîne répétée avec le bon format
message = f"Я больше никогда не буду писать \"{phrase}\"!"
resultat = (message + '\n') * nomber_rep

# Affichage du résultat
print(resultat.strip())
```
### J.Деловая колбаса
```
nomber_rep = int(input())  # Nombre de répétitions
phrase = input()  # Phrase à répéter

# Création de la chaîne répétée avec le bon format
message = f"Я больше никогда не буду писать \"{phrase}\"!"
resultat = (message + '\n') * nomber_rep

# Affichage du résultat
print(resultat)
```
### K.Автоматизация игры
```
nb_child = int(input())
nb_kal = int(input())
k = nb_child * nb_kal // 2 
print(k)
```
### L.Интересное сложение
```
## Lecture des deux nombres
num1, num2 = input()[::-1], input()[::-1]

# Calcul et affichage du résultat
print(''.join(str((int(a) + int(b)) % 10) for a, b in zip(num1.ljust(3, '0'), num2.ljust(3, '0')))[::-1])
```
### M.Дед Мороз и конфеты
```
# Lecture des deux nombres
num1, num2 = input()[::-1], input()[::-1]

# Calcul et affichage du résultat
print(''.join(str((int(a) + int(b)) % 10) for a, b in zip(num1.ljust(3, '0'), num2.ljust(3, '0')))[::-1])
# Lecture des deux nombres
num1, num2 = input()[::-1], input()[::-1]

# Calcul et affichage du résultat
print(''.join(str((int(a) + int(b)) % 10) for a, b in zip(num1.ljust(3, '0'), num2.ljust(3, '0')))[::-1])

```
### N.Шарики и ручки
```
num_enfant = int(input())
num_konf = int(input())
nb_dis = str(num_konf // num_enfant)
rest = num_konf % num_enfant
print(nb_dis)
print(rest)
```
### O.В ожидании доставки
```
red = int(input())
green = int(input())
blue = int(input())
print(red + blue + 1)

```
### P.Доставка
```
time_1 = int(input())
time_2 = int(input())
time_f = int(input())
minute = str((time_2 + time_f) % 60)
hours = str((time_1 + (time_2 + time_f) // 60) % 24)
print(f'{hours.rjust(2, "0")}:{minute.rjust(2, "0")}')

```
### Q.Ошибка кассового аппарата
```
distance1 = int(input())
distance_2 = int(input())
vitesse = int(input())
time_exact = abs(distance1 - distance_2) / vitesse
print(f"{time_exact:.2f}")
```
### R.Сдача 10
```
somme_dec = int(input())
somme_bin = input()
convert = int(somme_bin, 2)
print(somme_dec + convert)
```
### S.Украшение чека
```
name_pro, price, weight, my_wallet = input(), int(input()), int(input()), int(input())
liste = ["Товар:", "Цена:", "Итого:", "Внесено:", "Сдача:"]
values = [
    name_pro,
    f'{weight}кг * {price}руб/кг',
    f'{price * weight}руб',
    f'{my_wallet}руб',
    f'{my_wallet - price * weight}руб'
]
print('Чек'.center(35, "="))
for i in range(len(liste)):
    print(f"{liste[i]:<15}{values[i]:>20}")
print('=' * 35)
```
### T.Мухи отдельно, котлеты отдельно
```
weight, price, price_1, price_2 = int(input()), int(input()), int(input()), int(input())
weight_1 = int((price - price_2) * weight / (price_1 - price_2))
weight_2 = weight - weight_1
print(weight_1, weight_2)
```






























