# // day 1 of coding im starting to question my wellbeing

from random import randint # rand-randowmowa # int - jakaś liczba
result = 0
for row in rows:
    result += max(row)


ile = int(input("Ile liczb wylosować? "))
lista = []
for i in range(ile):
    lista.append(randint(-10, 10))
    if sum(lista) == 0:
        print("podane liczby spełniają warunki zadania") # kończy funkcje \\ nie może być
        return result

    print(lista)

# // looking horibble king

# // coś tam było jeszcze kodowane ale to do kosza beznadzieje stara czasu wgl a 3.0 <3


# // Final code i quess?

def sub_lists (l):
    lists = list()
    for i in range(len(l) + 1):
        for j in range(i):
            if sum(l[j: i])==0:
                lists.append(l[j: i])
    return lists
 

l1 = [3, 4, -7,3,1,3,1,-4,-2,-2]
print(sub_lists(l1))
