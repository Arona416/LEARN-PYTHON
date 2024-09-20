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
# Lecture des deux nombres
num1, num2 = input()[::-1], input()[::-1]

# Calcul et affichage du résultat
print(''.join(str((int(a) + int(b)) % 10) for a, b in zip(num1.ljust(3, '0'), num2.ljust(3, '0')))[::-1])
```



























