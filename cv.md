# Sergei Molokhvei

## Contacts
- +375299309709
- sergei.molohvey@gmail.com
- [Linkedin](https://www.linkedin.com/in/sergei-molokhvei-56b41b1aa/)

## Summary
I’d like to find a job and start working as a Junior front-end developer. Moreover, I’d like to learn React, Angular, NodeJS and other technologies. I enjoy studying and I’m ready to gain experience. I can work full time.

## Skills
- Python
- C++
- JavaScript

## Code examples
```Python
import random

score = 0
condition = None
while condition != '0':
    print(""" Здравствуйте и добро пожаловать в игру Анаграммы!
     Ваша задача: отгадать слово по буквам
     (Нажмите клавишу ввода, чтобы выйти.) """)
    maxscore = int(input('Введите максимальное количество очков которое вы хотите получить в итоге: '))
    while score < maxscore:
        WORDS = (
            "python", "анаграмма", "Пушкин", "rosa", "Гагарин", "intel", "шляпа", "процессор", "мак", "assembler",
            "банк", "volkswagen", "steam", "android", "ель", "человечность", "магазин", "пенал", "штопор", "ibm")
        word = random.choice(WORDS)
        correct = word
        jumble = ""
        while word:
            position = random.randrange(len(word))
            jumble += word[position]
            word = word[:position] + word[(position + 1):]
        print("Анаграмма: ", jumble)
        attemptsMax = int(input("Сколько вы хотите попыток?"))
        attemptsYour = 0
        guess = ""
        while attemptsYour < attemptsMax and guess != correct:
            if guess != correct:
                guess = input("Ваши догадки: ")
                if guess != correct:
                    print("Извините, не верно.")
            if guess == correct:
                print("Всё верно, Вы угадали!\n")
                score += 15
            if attemptsYour == attemptsMax:
                print("Извините, количество попыток исчерпано :(")
                break
            attemptsYour += 1
    print("Поздравляем с завершением игры!\nПолучено очков " + str(score) + ".\nСпасибо за игру.")
    condition = input("Если хотите играть снова, нажмите любую клавишу. Если хотите выйти, нажмите 0.")
    score = 0
```
## Experience 
No experience

## Education
Studying in Belarusian National Technical University, Information Technologies and Robotics faculty, Software for computers and automated systems.

## English level
My English level is B1 Intermediate (Epam test)
