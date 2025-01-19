#Vetor
aprendendo logica de programação com a linguagem visualg com o curso em video

algoritmo "Vetor"
var
m: vetor [1..4, 1..4] de inteiro
l,c, sDP, p2l, mn3: inteiro

inicio
    p2l <- 1
    para l <- 1 ate 4 faca
       para c <- 1 ate 4 faca
         escreva ("digite um numero para a posição[",l,",",c,"]")
         leia (m[l,c])
         se (l = c) entao
           sDP <- sDP + m[l,c]
         fimse
       fimpara
    fimpara
    para l <- 1 ate 4 faca
       para c <- 1 ate 4 faca
          escreva (m[l,c]:5)
       fimpara
         escreval ()
    fimpara
    para c <- 1 ate 4 faca
       p2l <- p2l * m[2,c]
    fimpara    
    para l <- 1 ate 4 faca
       se (m[l,3] > mn3) entao
         mn3 <- m[l,3]
       fimse
    fimpara
    escreval (" A soma da diagonal principal é: ", sDP)
    escreval (" A multiplicação da linha 2 é : ", p2l)
    escreval (" Maior numero da 3.a coluna: ", mn3)
    
fimalgoritmo
