 # Sorting in python
 s = input()
l = len(s)
for i in range(1, l):
    for j in range(0, l - i):
        if s[j] > s[j + 1]:
            ch = s[j]
            s = s[:j] + s[j + 1] + s[j + 2:]
            s = s[:j + 1] + ch + s[j + 1:]
