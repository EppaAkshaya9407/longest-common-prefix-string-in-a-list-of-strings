# longest-common-prefix-string-in-a-list-of-strings
n = int(input("Enter number of strings: "))
strs = []
for i in range(n):
    s = input("Enter string: ")
    strs.append(s)
res = ""
s1= strs[0]
n = len(s1)
for i in range(n):
    for s in strs:
        if i == len(s) or s[i] != s1[i]:
            print("Longest Common Prefix:", res)
            exit()
    res += s1[i]

print("Longest Common Prefix:", res)
