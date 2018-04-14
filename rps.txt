from random import choice

def RPS():
    options = ['Rock', 'Paper', 'Scissors']
    P1=choice(options)
    P2=choice(options)
    if P1 == P2:
        result = "DRAW"
    
    #P1 == Rock
    if P1 == 'Rock':
        if P2 == 'Paper':
            result = "P2 WON!"
        if P2 == 'Scissors':
            result = "P1 WON!"

    #P1 == Paper
    if P1 == 'Paper':
        if P2 == 'Rock':
            result = "P1 WON!"
        if P2 == 'Scissors':
            result = "P2 WON!"

    #P1 == Scissors
    if P1 == 'Scissors':
        if P2 == 'Rock':
            result = "P2 WON!"
        if P2 == 'Paper':
            result = "P1 WON!"
            
    return (P1, P2, result)

print(RPS());