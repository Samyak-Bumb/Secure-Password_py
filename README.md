# Secure-Password_py

```python
# Created By Samyak Bumb

SECURE = (
    # Total 27 Lines
    ('a', '@'),
    ('A', '@'),
    ('c', '('),
    ('C', '('),
    ('d', '(|'),
    ('D', '|)'),
    ('h', '|-|'),
    ('H', '|-|'),
    ('i', '1'),
    ('I', '!'),
    ('k', '|<'),
    ('K', '|<'),
    ('l', '|'),
    ('L', '|_'),
    ('M', '|\/|'),
    ('N', '|\|'),
    ('o', '0'),
    ('O', '()'),
    ('q', '?'),     # 'q' Word Means 'Why' in Marvari, Hindi for that '?' is Added (Samjh Me Aaya Kya)
    ('s', '$'),
    ('S', '$'),
    ('u', '|_|'),
    ('U', '|_|'),
    ('v', '\/'),
    ('V', '\/'),
    ('y', '-<'),
    ('Y', '-<'),
    ('and', '&')
)

def securePassword(password):
    for a, b in SECURE:
        password = password.replace(a, b)
    return password

if __name__ == "__main__":

    password = input("Enter your Password\n")
    password = securePassword(password)

    print(f"Congratulations Your Modified Password is  {password}")
```
