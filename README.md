def main():
    while True:
        print("\nВыберите функцию (1-10), или 0 для выхода:")
        print("1. Конкатенация (сложение строк)")
        print("2. Повторение строки")
        print("3. Обращение по индексу")
        print("4. Извлечение среза")
        print("5. Поиск подстроки (первое вхождение)")
        print("6. Поиск подстроки (последнее вхождение)")
        print("7. Замена шаблона")
        print("8. Разбиение строки по разделителю")
        print("9. Проверка состава строки (цифры/буквы/цифры+буквы)")
        print("10. Преобразование регистра")
        print("0. Выход")

        choice = input("Введите номер функции: ")

        if choice == "1":
            concatenate_strings()
        elif choice == "2":
            repeat_string()
        elif choice == "3":
            access_by_index()
        elif choice == "4":
            slice_string()
        elif choice == "5":
            find_substring_first()
        elif choice == "6":
            find_substring_last()
        elif choice == "7":
            replace_substring()
        elif choice == "8":
            split_string()
        elif choice == "9":
            check_string_composition()
        elif choice == "10":
            change_string_case()
        elif choice == "0":
            break
        else:
            print("Некорректный ввод. Попробуйте снова.")

def concatenate_strings():
    # Конкатенация (сложение строк)
    s1 = "Hello"
    s2 = " World"
    result = s1 + s2
    print("Результат конкатенации:", result)

def repeat_string():
    # Повторение строки
    s = "abc"
    result = s * 3
    print("Результат повторения строки:", result)

def access_by_index():
    # Обращение по индексу
    s = "Python"
    print("Символ с индексом 2:", s[2])

def slice_string():
    # Извлечение среза
    s = "Hello, World!"
    print("Срез от 3 до 8:", s[3:9])

def find_substring_first():
    # Поиск подстроки (первое вхождение)
    s = "Hello, World!"
    print("Первое вхождение 'World':", s.find("World"))

def find_substring_last():
    # Поиск подстроки (последнее вхождение)
    s = "Hello, World, World!"
    print("Последнее вхождение 'World':", s.rfind("World"))

def replace_substring():
    # Замена шаблона
    s = "Hello, World!"
    new_s = s.replace("World", "Python")
    print("Строка после замены:", new_s)

def split_string():
    # Разбиение строки по разделителю
    s = "apple,banana,cherry"
    fruits = s.split(",")
    print("Разделение по запятой:", fruits)

def check_string_composition():
    # Проверка состава строки (цифры/буквы/цифры+буквы)
    s = "123abc"
    print("Состоит ли из цифр:", s.isdigit())
    print("Состоит ли из букв:", s.isalpha())
    print("Состоит ли из цифр или букв:", s.isalnum())

def change_string_case():
    # Преобразование регистра
    s = "Hello, World!"
    print("В верхний регистр:", s.upper())
    print("В нижний регистр:", s.lower())

if __name__ == "__main__":
    main()
