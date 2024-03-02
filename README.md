# -Шеснадцатиричные числа, не превышающие 102410 расположенные в порядке убывания. Для каждой такой последовательности максимальное число вывести прописью.


with open('input.txt', 'r') as f:
    s = f.read(1024)
    if not s:
        print('the file is empty')
    n = s.split()
    print(n)
    for i in n:
        try:
            u = str(int(i, 16))
        except ValueError:
            print('does not satisfy the condition')
            continue
        print(i.lower())
        break
f.close()
