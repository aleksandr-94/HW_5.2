# HW_5.2


while True:
    number1 = float(input("Введите число "))
    number2 = float(input("Введите число "))
    operation = input("Выберите операцию(+, -, *, /):")
    if operation == "+":
        result = number1 + number2
        print("Результат:", result)
    elif operation == "-":
        result = number1 - number2
        print("Результат:", result)
    elif operation == "*":
        result = number1 * number2
        print("Результат:", result)
    elif operation == "/":
        if number2 == 0:
            print("Деление но 0 запрещено")
        else:
            result = number1 / number2
            print("Результат:", result)
    else:
        print("Операция неверная")
    continue_calc = input("Хотите продолжить? Введите 'yes': ")
    if continue_calc.lower() != 'yes':
        print('Завершено')
        break
