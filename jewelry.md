# Открытие файлов для чтения и записи
with open('input.txt', 'r') as input_file:
    j = input_file.readline().strip()
    s = input_file.readline().strip()

# Подсчёт символов из S, которые есть в J
count = sum(1 for ch in s if ch in j)

# Запись результата в output.txt
with open('output.txt', 'w') as output_file:
    output_file.write(str(count))
