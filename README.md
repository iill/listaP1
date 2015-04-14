"""Ola! Esse programa simula uma corrida de cavalos. """

path = players = 0 ## Variaveis usadas para definir os aspectos do jogo (jogadores e tamanho da corrida)

total1 = total2 = total3 = total4 = total5 = total6 = 0 ## Variaveis usadas para armazenar as 'casas andadas' pelos jogadores e determinar o vencedor.

player1 = player2 = player3 = player4 = player5 = player6 = 0 ## Variaveis usada para realizar a jogada dos players.

randomer = 0 ## Variavel usada para gerar o numero aleatorio.


print "Bem vindo a corrida de Cavalos!"
print "As regras sao simples: de um palpite num numero de 1 a 10 quando chegar sua vez e deseje para estar com sorte!"

import random

print
print

path = input("Por favor, informe o tamanho da sua corrida! ")
players = input("Informe o numero de jogadores que irao joga-la! ")

while path > 100 or path < 10:
    path = input("Informe novamente o tamanho da corrida. Deve ser um numero inteiro entre 10 e 100. ")

while players > 6 or players < 2:
    players = input("Voce precisa de no minimo 2 e no maximo 6 jogadores para a corrida! ")
print 


## Comandos para 2 jogadores.
 
    
if players == 2:
    

    while total1 < path and total2 < path:
            
        randomer = random.randint (1, 10)

        ## BLOCO DE ENTRADA DE JOGADAS

        player1 = input("Jogador 1, informe um numero de 1 a 10. ")

        while player1 < 1 or player1 > 10:
            player1 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player2 = input("Jogador 2, informe um numero de 1 a 10. ")

        while player2 < 1 or player2 > 10:
            player2 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")
        

        ## bloco de jogadas do Jogador 1
            
        if player1 == randomer:
            total1 = total1 + 10
            print "O cavalo 1 esta com sorte e correu 10 jardas!"
               
        if player1 != randomer:
            
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1 == 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O cavalo 1 esta cansado e trotou 5 jardas!" 

            else:
                total1 = total1 + 1
                print "O cavalo 1 esta com sono e andou apenas 1 jarda..."
        

        ## Bloco de jogadas do jogador 2

        if player2 == randomer:
            total2 = total2 + 10
            print "O cavalo 2 esta com sorte e correu 10 jardas!"
                
        if player2 != randomer:

            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2 == 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O cavalo 2 esta cansado e trotou 5 jardas!"
            
            else:
                total2 = total2 + 1
                print "O cavalo 2 esta com sono e andou apenas 1 jarda..."


## Comandos para 3 jogadores

            
if players == 3:

    while total1 < path and total2 < path and total3 < path:
            
        randomer = random.randint (1, 10)

        ## BLOCO DE ENTRADA DE JOGADAS

        player1 = input("Jogador 1, informe um numero de 1 a 10. ")
        
        while player1 < 1 or player1 > 10:
            player1 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player2 = input("Jogador 2, informe um numero de 1 a 10. ")
        
        while player2 < 1 or player2 > 10:
            player2 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")
        
        player3 = input("Jogador 3, informe um numero de 1 a 10. ")
        
        while player3 < 1 or player3 > 10:
            player3 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")
        

        ## Bloco de jogadas do jogador 1

        if player1 == randomer:
            total1 = total1 + 10
            print "O cavalo 1 esta com sorte e correu 10 jardas!"
               
        if player1 != randomer:
            
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1 == 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O cavalo 1 esta cansado e trotou 5 jardas!" 

            else:
                total1 = total1 + 1
                print "O cavalo 1 esta com sono e andou apenas 1 jarda..."
        

        ## Bloco de jogadas do jogador 2
            
        if player2 == randomer:
            total2 = total2 + 10
            print "O cavalo 2 esta com sorte e correu 10 jardas!"
                
        if player2 != randomer:

            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2 == 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O cavalo 2 esta cansado e trotou 5 jardas!"
            
            else:
                total2 = total2 + 1
                print "O cavalo 2 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 3
            
        if player3 == randomer:
            total3 = total3 + 10
            print "O cavalo 3 esta com sorte e correu 10 jardas!"
                
        if player3 != randomer:

            if player3 - randomer == 2 or randomer - player3 == 2 or randomer - player3 == 1 or player3 - randomer == 1:
                total3 = total3 + 5
                print "O cavalo 3 esta cansado e trotou 5 jardas!"
            
            else:
                total3 = total3 + 1
                print "O cavalo 3 esta com sono e andou apenas 1 jarda..."


## Comandos para 4 jogadores

            
if players == 4:

    while total1 < path and total2 < path and total3 < path and total4 < path:
            
        randomer = random.randint (1, 10)
        
        ## BLOCO DE ENTRADA DE JOGADAS

        player1 = input("Jogador 1, informe um numero de 1 a 10. ")
        
        while player1 < 1 or player1 > 10:
            player1 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player2 = input("Jogador 2, informe um numero de 1 a 10. ")
        
        while player2 < 1 or player2 > 10:
            player2 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player3 = input("Jogador 3, informe um numero de 1 a 10. ")
        
        while player3 < 1 or player3 > 10:
            player3 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player4 = input("Jogador 4, informe um numero de 1 a 10. ")
        
        while player4 < 1 or player4 > 10:
            player4 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")
            
        
        ## bloco de jogadas do Jogador 1.

        if player1 == randomer:
            total1 = total1 + 10
            print "O cavalo 1 esta com sorte e correu 10 jardas!"
               
        if player1 != randomer:
            
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1 == 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O cavalo 1 esta cansado e trotou 5 jardas!" 

            else:
                total1 = total1 + 1
                print "O cavalo 1 esta com sono e andou apenas 1 jarda..."
        

        ## Bloco de jogadas do jogador 2

        if player2 == randomer:
            total2 = total2 + 10
            print "O cavalo 2 esta com sorte e correu 10 jardas!"
                
        if player2 != randomer:

            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2 == 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O cavalo 2 esta cansado e trotou 5 jardas!"
            
            else:
                total2 = total2 + 1
                print "O cavalo 2 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 3
            
        if player3 == randomer:
            total3 = total3 + 10
            print "O cavalo 3 esta com sorte e correu 10 jardas!"
                
        if player3 != randomer:

            if player3 - randomer == 2 or randomer - player3 == 2 or randomer - player3 == 1 or player3 - randomer == 1:
                total3 = total3 + 5
                print "O cavalo 3 esta cansado e trotou 5 jardas!"
            
            else:
                total3 = total3 + 1
                print "O cavalo 3 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 4
            
        if player4 == randomer:
            total4 = total4 + 10
            print "O cavalo 4 esta com sorte e correu 10 jardas!"
                
        if player4 != randomer:

            if player4 - randomer == 2 or randomer - player4 == 2 or randomer - player4 == 1 or player4 - randomer == 1:
                total4 = total4 + 5
                print "O cavalo 4 esta cansado e trotou 5 jardas!"
            
            else:
                total4 = total4 + 1
                print "O cavalo 4 esta com sono e andou apenas 1 jarda..."
             

## Comandos para 5 jogadores

            
if players == 5:

    while total1 < path and total2 < path and total3 < path and total4 < path and total5 < path:
            
        randomer = random.randint (1, 10)


        ## BLOCO DE ENTRADA DE JOGADAS

        player1 = input("Jogador 1, informe um numero de 1 a 10. ")
        
        while player1 < 1 or player1 > 10:
            player1 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player2 = input("Jogador 2, informe um numero de 1 a 10. ")
        
        while player2 < 1 or player2 > 10:
            player2 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player3 = input("Jogador 3, informe um numero de 1 a 10. ")
        
        while player3 < 1 or player3 > 10:
            player3 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player4 = input("Jogador 4, informe um numero de 1 a 10. ")
        
        while player4 < 1 or player4 > 10:
            player4 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player5 = input("Jogador 5, informe um numero de 1 a 10. ")
        
        while player5 < 1 or player5 > 10:
            player5 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")


        ## bloco de jogadas do Jogador 1.
            
        if player1 == randomer:
            total1 = total1 + 10
            print "O cavalo 1 esta com sorte e correu 10 jardas!"
               
        if player1 != randomer:
            
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1 == 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O cavalo 1 esta cansado e trotou 5 jardas!" 

            else:
                total1 = total1 + 1
                print "O cavalo 1 esta com sono e andou apenas 1 jarda..."
        

        ## Bloco de jogadas do jogador 2
            
        if player2 == randomer:
            total2 = total2 + 10
            print "O cavalo 2 esta com sorte e correu 10 jardas!"
                
        if player2 != randomer:

            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2 == 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O cavalo 2 esta cansado e trotou 5 jardas!"
            
            else:
                total2 = total2 + 1
                print "O cavalo 2 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 3

        if player3 == randomer:
            total3 = total3 + 10
            print "O cavalo 3 esta com sorte e correu 10 jardas!"
                
        if player3 != randomer:

            if player3 - randomer == 2 or randomer - player3 == 2 or randomer - player3 == 1 or player3 - randomer == 1:
                total3 = total3 + 5
                print "O cavalo 3 esta cansado e trotou 5 jardas!"
            
            else:
                total3 = total3 + 1
                print "O cavalo 3 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 4

        if player4 == randomer:
            total4 = total4 + 10
            print "O cavalo 4 esta com sorte e correu 10 jardas!"
                
        if player4 != randomer:

            if player4 - randomer == 2 or randomer - player4 == 2 or randomer - player4 == 1 or player4 - randomer == 1:
                total4 = total4 + 5
                print "O cavalo 4 esta cansado e trotou 5 jardas!"
            
            else:
                total4 = total4 + 1
                print "O cavalo 4 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 5

        if player5 == randomer:
            total5 = total5 + 10
            print "O cavalo 5 esta com sorte e correu 10 jardas!"
                
        if player5 != randomer:

            if player5 - randomer == 2 or randomer - player5 == 2 or randomer - player5 == 1 or player5 - randomer == 1:
                total5 = total5 + 5
                print "O cavalo 5 esta cansado e trotou 5 jardas!"
            
            else:
                total5 = total5 + 1
                print "O cavalo 5 esta com sono e andou apenas 1 jarda..."


## Comandos para 6 jogadores

            
if players == 6:

    while total1 < path and total2 < path and total3 < path and total4 < path and total5 < path and total6 < path:
            
        randomer = random.randint (1, 10)
        

        ## BLOCO DE ENTRADA DE JOGADAS

        player1 = input("Jogador 1, informe um numero de 1 a 10. ")
        
        while player1 < 1 or player1 > 10:
            player1 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player2 = input("Jogador 2, informe um numero de 1 a 10. ")
        
        while player2 < 1 or player2 > 10:
            player2 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player3 = input("Jogador 3, informe um numero de 1 a 10. ")
        
        while player3 < 1 or player3 > 10:
            player3 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player4 = input("Jogador 4, informe um numero de 1 a 10. ")
        
        while player4 < 1 or player4 > 10:
            player4 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player5 = input("Jogador 5, informe um numero de 1 a 10. ")
        
        while player5 < 1 or player5 > 10:
            player5 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")

        player6 = input("Jogador 6, informe um numero de 1 a 10. ")
        
        while player6 < 1 or player6 > 10:
            player6 = input("Entrada invalida! Por favor informe um numero inteiro entre 1 e 10. ")
            
           
       

        ## Bloco de jogadas do Jogador 1.

        if player1 == randomer:
            total1 = total1 + 10
            print "O cavalo 1 esta com sorte e correu 10 jardas!"
               
        if player1 != randomer:
            
            if player1 - randomer == 2 or randomer - player1 == 2 or randomer - player1 == 1 or player1 - randomer == 1:
                total1 = total1 + 5
                print "O cavalo 1 esta cansado e trotou 5 jardas!" 

            else:
                total1 = total1 + 1
                print "O cavalo 1 esta com sono e andou apenas 1 jarda..."
        

        ## Bloco de jogadas do jogador 2

        if player2 == randomer:
            total2 = total2 + 10
            print "O cavalo 2 esta com sorte e correu 10 jardas!"
                
        if player2 != randomer:

            if player2 - randomer == 2 or randomer - player2 == 2 or randomer - player2 == 1 or player2 - randomer == 1:
                total2 = total2 + 5
                print "O cavalo 2 esta cansado e trotou 5 jardas!"
            
            else:
                total2 = total2 + 1
                print "O cavalo 2 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 3

        if player3 == randomer:
            total3 = total3 + 10
            print "O cavalo 3 esta com sorte e correu 10 jardas!"
                
        if player3 != randomer:

            if player3 - randomer == 2 or randomer - player3 == 2 or randomer - player3 == 1 or player3 - randomer == 1:
                total3 = total3 + 5
                print "O cavalo 3 esta cansado e trotou 5 jardas!"
            
            else:
                total3 = total3 + 1
                print "O cavalo 3 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 4

        if player4 == randomer:
            total4 = total4 + 10
            print "O cavalo 4 esta com sorte e correu 10 jardas!"
                
        if player4 != randomer:

            if player4 - randomer == 2 or randomer - player4 == 2 or randomer - player4 == 1 or player4 - randomer == 1:
                total4 = total4 + 5
                print "O cavalo 4 esta cansado e trotou 5 jardas!"
            
            else:
                total4 = total4 + 1
                print "O cavalo 4 esta com sono e andou apenas 1 jarda..."


        ## Bloco de jogadas do jogador 5

        if player5 == randomer:
            total5 = total5 + 10
            print "O cavalo 5 esta com sorte e correu 10 jardas!"
                
        if player5 != randomer:

            if player5 - randomer == 2 or randomer - player5 == 2 or randomer - player5 == 1 or player5 - randomer == 1:
                total5 = total5 + 5
                print "O cavalo 5 esta cansado e trotou 5 jardas!"
            
            else:
                total5 = total5 + 1
                print "O cavalo 5 esta com sono e andou apenas 1 jarda..."


         ## Bloco de jogadas do jogador 6

        if player6 == randomer:
            total6 = total6 + 10
            print "O cavalo 6 esta com sorte e correu 10 jardas!"
                
        if player6 != randomer:

            if player6 - randomer == 2 or randomer - player6 == 2 or randomer - player6 == 1 or player6 - randomer == 1:
                total6 = total6 + 5
                print "O cavalo 6 esta cansado e trotou 5 jardas!"
            
            else:
                total6 = total6 + 1
                print "O cavalo 6 esta com sono e andou apenas 1 jarda..."


## Resultado 


if total1 >= path:
    print 
    print "Parabens! O Jogador 1 venceu a corrida!"
        
if total2 >= path:
    print 
    print "Parabens! O Jogador 2 venceu a corrida!"

if total3 >= path:
    print 
    print "Parabens! O Jogador 3 venceu a corrida!"

if total4 >= path:
    print 
    print "Parabens! O Jogador 4 venceu a corrida!"

if total5 >= path:
    print 
    print "Parabens! O Jogador 5 venceu a corrida!"

if total6 >= path:
    print 
    print "Parabens! O Jogador 6 venceu a corrida!"
