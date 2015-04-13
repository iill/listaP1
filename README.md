# listaP1

print "Bem vindo à corrida dos Patifes!"

path = input("Informe o tamanho da sua corrida!")
players = input("Informe o número de Patifes que irão jogá-la!")

while path > 100 or path < 10:
    path = input("Informe novamente o tamanho da corrida. Deve ser um número entre 10 e 100.")

while players > 6 or players < 2:
    players = input("Você precisa de no mínimo 2 e no máximo 6 patifes para a corrida!")
    
##RODADA 1 

import random

def rodada(jog):
    total1 = 0
    total2 = 0
    
    if jog == 2:
        while total1 != path or total2 != path:
            
            randomer = randint (1, 10)
            
            player1 = input("Patife 1, informe um número de 1 a 10")
            if player1 == randomer:
                total1 = total1 + 10
                print "O Patife 1 
            
                
            
            
            player2 = input("Patife 2, informe um número de 1 a 10")
    
    
    
if players = 2


