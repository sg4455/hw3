# hw3
def binary(num):
    print(bin(num))


def ascii(charlist):
    mystring = ""
    for char in charlist:
        mystring = mystring + chr(char)
    print mystring

def binToHex(num):
    print hex(int(num, 2))

def oct(num):
    index = 0
    digit = 0
    while num != 0:
        remainder = num % 10 
        num = num / 10
        digit = (remainder * 8**index) + digit
        index= index +1
    print digit
    
list = [0x57, 0x68 ,0x61 ,0x74 ,0x20 ,0x74 ,0x68 ,0x65 ,0x20 ,0x68 ,0x65 ,0x78 ,0x3f]
ascii(list)
binToHex('11111111111111111001000001100010')
oct(77)
oct(113)
