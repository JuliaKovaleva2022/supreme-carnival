# supreme-carnival
Задание 1

word=str(input("Напишите слово: "))
n=len (word)//2
if len (word) % 2 == 0:
        print(word [n-1:n+1])
else:
       print(word[n]) 
# или print(word[int (len(word)/2 - 0.1)])

Задание 2
a = int(input("введите число: "))
b = 0
while a:
    b += a
    a = int(input("введите число: "))
print (b)

Задание 3
Вариант с парами:
boys = ['Peter','Alex', 'John', 'Arthur', 'Richard']
girls = ['Kate', 'Liza', 'Kira', 'Emma', 'Trisha']
if len(boys)==len(girls):
    print("Идеальная пара:")
    boys.sort()
    girls.sort()
    dating = zip(boys, girls)
    for company in dating:
        print(f"{company[0]} и {company[1]}")
else:
 
    print("Кто то может остаться без пары")
    
Вариант без пар:

   boys = ['Peter', 'Alex', 'John', 'Arthur', 'Richard', 'Michael']
girls = ['Kate', 'Liza', 'Kira', 'Emma', 'Trisha']
if len(boys)==len(girls):
    print("Идеальная пара:")
    boys.sort()
    girls.sort()
    dating = zip(boys, girls)
    for company in dating:
        print(f"{company[0]} и {company[1]}")
else:
 
    print("Кто то может остаться без пары")
    
Задание 4
countries_temperature = [
    ['Thailand', [75.2, 77, 78.8, 73.4, 68, 75.2, 77]],
    ['Germany', [57.2, 55.4, 59, 59, 53.6]],
    ['Russia', [35.6, 37.4, 39.2, 41, 42.8, 39.2, 35.6]],
    ['Poland', [50, 50, 53.6, 57.2, 55.4, 55.4]]
]
for i in countries_temperature:
    print(i[0], '-', round((sum(i[1]) / len(i[1]) - 32) / 1.8, 1), 'C')
