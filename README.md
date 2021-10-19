# hello-world
Just another repository

Пока что побудет здесь:

def to_number(s):
    my_string = [c.upper() for c in s]

    my_dict = {'1':	'.,?!:',
           '2': 'ABC',
           '3': 'DEF',
           '4': 'GHI',
           '5': 'JKL',
           '6': 'MNO',
           '7': 'PQRS',
           '8': 'TUV',
           '9': 'WXYZ',
           '0': ' '}
           
    for c in my_string:
        for values in my_dict:
            if c in my_dict[values]:
                print(values * (my_dict[values].index(c) + 1), end='')
            

print("Please input your request in English")
s = input()
print('Result:')
to_number(s)
