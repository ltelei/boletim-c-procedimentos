# boletim-c-procedimentos[08:58, 25/04/2023] Lucas Nepomuceno: henriqueodevelp@gmail.com
pR0GR4m@tH0r
[22:11, 25/04/2023] Lucas Nepomuceno: Algoritmo "25/04"
//
//
//
//
// Descrição   : Aqui você descreve o que o programa faz! (função)
// Autor(a)    : Nome do(a) aluno(a)
// Data atual  : 25/04/2023

tipo
   estudante = registro
      nome: caractere
      idade: inteiro
    x,  nota1,nota2,nota3,nota4, media: real
   fimregistro





procedimento menu()
var
   cadastro: caracter
   op : inteiro
inicio

   enquanto op <> 9 faca
      escreval("========== MENU ==========")
      escreval(" 1 - cadastro ")
      escreval(" 2 - lancar nota ")
      escreval(" 3 - imprimir diário")
      escreval("==========================")
      escreva("op >")
      leia(op)


      escolha op

      caso 1
         cadastro()
      caso 2
         lancarnotas()
      caso 3
         imprimirdiario()
      outrocaso
         escreval("saindo ...")
      outrocaso
         escreval("opçao invalida")
      fimescolha
   fimenquanto
fimprocedimento


procedimento cadastro()      // cadastrando alunos
var
   op1: caractere
inicio
   qtd_aluno <-qtd_aluno+1
   Escreval ("Digite o nome do aluno ", qtd_aluno)
   leia (alunos[qtd_aluno].nome)
   Escreval ("Digite a idade do aluno ", qtd_aluno)
   leia (alunos[qtd_aluno].idade)
   Escreval (" Aluno cadastrado com sucesso, deseja continuar S / N?")
   leia (op1)
   se (op1 = "s") entao
      cadastro()

   fimse

fimprocedimento


procedimento lancarnotas()   //lançando notas
var
   op1 :caractere
inicio

   Escreval ("Digite o nome do aluno que deseja lançar a nota ")
   leia (alunos[qtd_aluno].nome)
   Escreval("Digite o valor da nota 1")
   leia (alunos[qtd_aluno].nota1)
   Escreval("Digite o valor da nota 2")
   leia (alunos[qtd_aluno].nota2)
   Escreval("Digite o valor da nota 3")
   leia (alunos[qtd_aluno].nota3)
   Escreval("Digite o valor da nota 4")
   leia (alunos[qtd_aluno].nota4)
   Escreval (" Nota lançada com sucesso, deseja contuinuar?")
   leia (op1)
   se (op1 = "s") entao
      lancarnotas()

   fimse
fimprocedimento



procedimento imprimirdiario()
var
media: real
inicio
para x de 1 ate qtd_alunos faca
Escreval(alunos[x].nome, " Notas : ", alunos[x].nota1," ", alunos[x].nota2," ", alunos[x].nota3," ", alunos[x].nota4," ", alunos[x].media)
escreval()
fimpara
fimprocedimento



 Var //Variaveis globais
   alunos : vetor [1..4] de estudante
   qtd_aluno : inteiro
   lancarnotas: vetor [1..4] de real
   cadastro: caracter
   imprimir_diario,nota,media: real



Inicio
   // Seção de Comandos, procedimento, funções, operadores, etc...

   menu()






fimalgoritmo
