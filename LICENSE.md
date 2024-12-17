def check_inequalities():
    while True:
        try:
            A = int(input("Введите целое число A: "))
            B = int(input("Введите целое число B: "))
            
            # Проверка неравенств
            if A > 2 and B < 3:
                print(f"Высказывание истинно: A = {A}, B = {B} -> A > 2 и B < 3.")
            else:
                print(f"Высказывание ложно: A = {A}, B = {B}.")
            
            # Предложение продолжить
            continue_check = input("Хотите проверить еще? (да/нет): ").strip().lower()
            if continue_check != 'да':
                break  # Выход из цикла, если пользователь не хочет продолжать
        except ValueError:
            print("Неправильно ввели! Пожалуйста, введите целые числа.")

check_inequalities()
def determine_color():
    while True:
        try:
            wavelength = float(input("Введите длину волны в нанометрах (нм): "))
            
            # Определение цвета в зависимости от длины волны
            if 620 <= wavelength <= 750:
                color = "Красный"
            elif 590 <= wavelength < 620:
                color = "Оранжевый"
            elif 570 <= wavelength < 590:
                color = "Желтый"
            elif 495 <= wavelength < 570:
                color = "Зеленый"
            elif 450 <= wavelength < 495:
                color = "Голубой"
            elif 380 <= wavelength < 450:
                color = "Фиолетовый"
            else:
                color = "Длина волны вне видимого спектра."
            
            print(f"Для длины волны {wavelength} нм, цвет: {color}")
            
            # Предложение продолжить
            continue_check = input("Хотите проверить еще? (да/нет): ").strip().lower()
            if continue_check != 'да':
                break  # Выход из цикла, если пользователь не хочет продолжать
        except ValueError:
            print("Неправильно ввели! Пожалуйста, введите числовое значение.")

determine_color()
