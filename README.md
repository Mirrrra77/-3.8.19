n=int(input("Количество билетов"))
b=0 #объявляем переменную, которая будет хранить сумму билетов, которые купят посетители
b1=0 #переменная с ценой на билеты
b2=90 #переменная с ценой на билеты
b3=1390 #переменная с ценой на билеты
for i in range(n): #цикл, в котором будет столько итераций, сколько билетов ввели с клавиатуры
    age = int(input("Возраст"))
    if  18 > age:
        b = b + b1
    elif 18 < age < 25:
        b = b + b2
    elif  25 < age:
        b = b + b3
if n > 3:
    b = b * (1-0.1)
print(b)
