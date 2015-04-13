print "Bem vindo à corrida dos Patifes!"

path = input("Informe o tamanho da sua corrida! ")
players = input("Informe o número de Patifes que irão jogá-la! ")

while path > 100 or path < 10:
    path = input("Informe novamente o tamanho da corrida. Deve ser um número entre 10 e 100. ")

while players > 6 or players < 2:
    players = input("Você precisa de no mínimo 2 e no máximo 6 patifes para a corrida! ")
    
##RODADA 1 

import random

def rodada(jog):
    total1 = 0
    total2 = 0
    
    if jog == 2:
        while total1 != path or total2 != path:
            
            randomer = random.randint (1, 10)
            
            player1 = input("Patife 1, informe um número de 1 a 10. ")
            
            while player1 < 1 or player1 > 10:
                player1 = input("Entrada inválida! Por favor informe um número entre 1 e 10")
            
            if player1 == randomer:
                total1 = total1 + 10
                print "O Patife 1 está com sorte e correu 10 espaços!"
                
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1== 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O Patife 1 está com preguiça e trotou 5 espaços!"
            
            else:
                total1 = total1 + 1
                print "O Patife 1 está com sono e andou apenas 1 espaço..."
            
            player2 = input("Patife 2, informe um número de 1 a 10")
            
            while player2 < 1 or player2 > 10:
                player2 = input("Entrada inválida! Por favor informe um número entre 1 e 10")
            if player2 == randomer:
                total2 = total2 + 10
                print "O Patife 2 está com sorte e correu 10 espaços!"
                
            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2== 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O Patife 2 está com preguiça e trotou 5 espaços!"
            
            else:
                total2 = total2 + 1
                print "O Patife 2 está com sono e andou apenas 1 espaço..."
        
        if total1 >= path:
            print "O Patife 1 venceu a corrida!"
        
        if total2 >= path:
            print "O Patife 2 venceu a corrida!"
            
    
