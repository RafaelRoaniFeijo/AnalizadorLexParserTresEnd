Yacc ( Yet Another Compiler-Compiler ) é um programa de computador para o sistema operacional Unix desenvolvido por Stephen C. Johnson . É um gerador de parser Look Ahead Left-to-Right Rightmost Derivation (LALR) , gerando um analisador LALR (a parte de um compilador que tenta fazer sentido sintático do código-fonte ) baseado em uma gramática formal , escrita em uma notação semelhante à Forma Backus–Naur (BNF) .Yacc é fornecido como um utilitário padrão no BSD e AT&T Unix. Linux baseado em GNUdistribuições incluem Bison , um substituto Yacc compatível com versões anteriores.

Bison , é um gerador de parser que faz parte do Projeto GNU . Bison lê uma especificação na notação BNF (uma linguagem livre de contexto ), 

Flex , um analisador léxico automático, é frequentemente usado com o Bison, para tokenizar dados de entrada e fornecer tokens ao Bison.
# Compilador
O front-end de um compilador que converte código python em código de três endereços (TAC).

### Instalação
Para instalar o Flex e o Bison execute os comandos abaixo em um terminal
```
$ sudo apt-get update
$ sudo apt-get install flex
$ sudo apt-get install bison
```

### Para rodar
Após instalar o Flex e o Bison siga os comandos abaixo:
```
$ bison -d parser.y
$ flex lexical.l
$ gcc lex.yy.c parser.tab.c -o compilador
$ ./compilador < ./data/input/input1.txt | cat > ./data/output/output1.txt
 ou 

 $ make all
```

To run the tests, execute the command: 
``` 
$ make test
```