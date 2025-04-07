import sys

# Чтение строк J и S
j = sys.stdin.readline().strip()
s = sys.stdin.readline().strip()

# Подсчёт символов из S, которые есть в J
count = sum(1 for ch in s if ch in j)

# Вывод результата
print(count)