score = 0
total_questions = 5

print("Вітаю в грі-вікторині!")
print("Відповідай на запитання і перевір свої знання!")
print("-" * 40)


answer1 = input("1. Хто був першим президентом України? ")
if answer1 == "Кравчук":
    print("Правильно! Молодець!")
    score += 1
else:
    print("Неправильно. Правильна відповідь: Кравчук")


answer2 = input("2. Яка найбільша тварина на планеті? ")
if answer2.lower() == "кит":
    print("Правильно! Молодець!")
    score += 1
else:
    print("Неправильно. Правильна відповідь: кит")


print("3. Скільки гравців у футбольній команді?")
print("а) 9   б) 10   в) 11   г) 12")
answer3 = input("Ваша відповідь (а/б/в/г): ")
if answer3 == "в":
    print("Правильно! Молодець!")
    score += 1
else:
    print("Неправильно. Правильна відповідь: в (11)")


answer4 = input("4. гори є, але плоскі, море є, але сухе? ")
if "карта" in answer4.lower() or "землю" in answer4.lower():
    print("Правильно! цеж ізі? :)")
    score += 1
else:
    print("Неправильно. Відповідь: карта")


answer5 = input("5. Хто написав «Кобзар»? ")
if answer5.lower() == "Шевченко" or "Тарас Шевченко" in answer5.lower():
    print("Правильно! Молодець!")
    score += 1
else:
    print("Неправильно. Відповідь: Тарас Шевченко")


print("-" * 40)
print(f"Гру завершено! Ви відповіли правильно на {score} з {total_questions} питань.")
if score == total_questions:
    print("Ти геній!")
elif score >= total_questions / 2:
    print("Непогано! Але є куди рости.")
else:
    print("Спробуй ще раз, буде краще!")
