Проект: Расчет средних значений выборки на Python

Описание: Этот проект реализует простой скрипт для вычисления среднего значения набора чисел, введенных пользователем. Программа написана на языке Python и позволяет легко взаимодействовать с пользователем.

Функционал:
Пользователь может вводить числа, отправляя их в программу.
Для завершения ввода пользователь может ввести 'q'.
Программа выводит среднее значение введенных чисел.


Код:
def calculate_average(numbers): if len(numbers) == 0: return 0 return sum(numbers) / len(numbers)

def main(): print("Введите числа (для завершения введите 'q'):") numbers = []

while True:

    user_input = input()
		
    if user_input.lower() == 'q':
		
        break
				
    try:
		
        number = float(user_input)
				
        numbers.append(number)
				
    except ValueError:
		
        print("Пожалуйста, введите число или 'q' для завершения.")
				
average = calculate_average(numbers)

print(f"Среднее значение выборки: {average}")

if name == "main": main()

Установка:
Убедитесь, что у вас установлен Python версии 3.6 и выше.
Скопируйте код в файл с именем average_calculator.py.

Использование:

1.Откройте терминал или командную строку.

2. Перейдите в директорию, где находится ваш файл average_calculator

3. Запустите программу: python average_calculator

4. Вводите числа, нажимая Enter после каждого.

5. Чтобы завершить ввод, введите 'q'.
