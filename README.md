#+Title: Aula 05
#+Author: Hugo Macedo

* Interação com o interpretador 
 - Comandos básicos 
  (load "ficheiro.lisp"), (quit)
 - Erros e usabilidade

* Uso do Emacs para interagir com o interpretador
 - Rodando o SLIME
 - Comandos de avaliação 

* Avaliando expressões
 - Números 
   - 1, 0, #c(1 2), ...
 - Símbolos
   - T, pi, ...
   - Strings "Isto é uma string"
 - S-expressions (op arg_1 arg_2 ... arg_n)
   - (+ 1 2), (sqrt -1), ...
 - Interrompendo a avaliação 
   - (quote Intervalo)
   - Operações especiais setf, quit, load,... 
 - Listas 
   - O operador list
   - Heterogeneidade das listas
   
* A dualidade programa/dados vs LISP
   - Questão de alunos (Para que serve o quote?)
     
     - O quote serve como forma de forçar o interpretador a tratar
       expressões como se fossem dados, ou seja símbolos/sintaxe não
       avaliável cuja semântica passa a ser o símbolo ele mesmo.

       Por exemplo, após avaliar a expressão (setf X 10), ao
       avaliar o simbolo X obtém-se 10 como resultado. Já ao
       avaliar 'X obtém-se X. 
     

* Dialectos do LISP
  - Common Lisp (Que usaremos ao longo do curso)
  - Scheme (Que usado em várias referências ex.: [[https://mitpress.mit.edu/sicp/][Structure and Interpretation of Computer Programs]] (SICP))
  - ELisp (Emacs Lisp)


* "Lição de casa"
 - Exercitar interação com interpretador via Emacs
 - [[https://guides.github.com/activities/hello-world/][GitHub Hello World]] 
  
