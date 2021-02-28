#Простой чат бот 
В этом репозитории лежит проект, который я написала как один из проектов академии JetBrains.  
Постановка задачи:  
>Here, at the beginning of your programmer’s path, creating a simple console chat bot will do wonders to guide you through the basics of coding. During this journey you will also play some word and number games that you are going to implement all on your own. Pack up and let’s hit the road, my friend!

Код:
``` Python
def greet(bot_name, birth_year):
    print('Hello! My name is ' + bot_name + '.')
    print('I was created in ' + birth_year + '.')


def remind_name():
    print('Please, remind me your name.')
    name = input()
    print('What a great name you have, ' + name + '!')


def guess_age():
    print('Let me guess your age.')
    print('Enter remainders of dividing your age by 3, 5 and 7.')

    rem3 = int(input())
    rem5 = int(input())
    rem7 = int(input())
    age = (rem3 * 70 + rem5 * 21 + rem7 * 15) % 105

    print("Your age is " + str(age) + "; that's a good time to start programming!")


def count():
    print('Now I will prove to you that I can count to any number you want.')

    num = int(input())
    curr = 0
    while curr <= num:
        print(curr, '!')
        curr = curr + 1


def test():
    print("Let's test your astronomical knowledge.")
    print("What's the name of the 8th planet of Solar System?")
    print("1. Jupiter\n2. Mars\n3. Neptune\n4. Venus")
    answer = int(input())
    if answer == 3:
        print("Completed, have a nice day!")
    else:
        print("Please, try again.")


def end():
    print('Congratulations, have a nice day!')


greet('Gray', '2021')
remind_name()
guess_age()
count()
test()
end()

```
