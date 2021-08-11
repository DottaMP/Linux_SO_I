# Linux_SO_I

### 1º semestre/2021 utilizando comandos com o *Ubuntu*    

Quebrando os códigos na Fatec, 2º semestre do curso de *Análise e Desenvolvimento de Sistemas*, disciplina Sistemas Operacionais I (*SO I*).   

##### Comandos do Linux
Who – mostra o usuário atual    
Date – mostra a data    
echo – mostra uma mensagem ou conteúdo de uma variável.    
Mensagem     
Echo “          “    
Variável    
echo $variável    

Chmod – atribui permissões    
Chmod ugo     
u- usuário    
g- grupo    
o- outros    
Permissões    
4 (Ler – r ): somente para visualizar o conteúdo do arquivo;    
2 (Gravar/Escrever - w): significa a possibilidade de edição do conteúdo;    
1 (Executar – x): autorização de rodar/executar um arquivo de programa ou script;    
0 (Sem permissão): ninguém pode alterar ou visualizar o arquivo, somente o proprietário pode ter alterar as permissões.    
Os três dígitos são representados da seguintes maneira:    
1º dígito= Usuário 2º dígito= Grupo 3º dígito= Público    
  
Para ver a permissão ls -l nomedo arquivo    
R= read    
W=write    
X=execution     

Edito de texto:    
Pico “nome do arquivo”    
Executar    
./ “nome do arquivo”     
    
Fazer um programa para escrever a mensagem “usuário atual” e exibir o nome do usuário e a mensagem “data e hora atual” e exibir a data e hora    
Sort $ n    
N= 0,1,2,3......    
Variável    
Nome=valor    
Mostrar     
echo $nome    
while [ condição]    
Programa    
#!/bin/sh    
nome=0    
while [ $nome -lt 10 ]    
do    
Mostra a variável    
nome=$((nome+1))    
done    
exit 0    
    
Passagem de parâmetros:    
./mostra arg1 arg2 arg3 ........    
$1 = arg1    
$2 = arg2    
$3 = arg3    
Comando if    
if [condição]    
then    
Comandos    
elif [condição]    
then    
 comandos    
elif .......    
else     
Comados    
fi    
    
Comparação Numérica:    
-lt	É menor que (LessThan)    
-gt	É maior que (GreaterThan)    
-le	É menor igual (LessEqual)    
-ge	É maior igual (GreaterEqual)    
-eq	É igual (EQual)    
-ne	É diferente (NotEqual)    
    
Comparação de Strings:    
=	É igual    
!=	É diferente    
-n	É não nula    
-z	É nula    
    
Operadores Lógicos :   
!	NÃO lógico (NOT)    
-a	E lógico (AND)    
-o	OU lógico (OR)    
   
Comando until (até que)    
until [ condição ]    
do    
Comandos    
Done    
    
Comando for    
for variável in <lista>    
do    
comandos    
done    
Lista:    
Exemplos:    
1 2 4 5     
$(seq 1 N)  $(seq 1 20)     
for contador $(seq 1 20)        
    
Break – encerra o laço     

Continue – salta para próxima interação    
    
if [condição]    
then    
Continue    
fi    
    
Comando case    
Case <variável> in    
<padrão>)    
Comandos;;    
<padrão>)    
Comandos;;     
<padrão>)    
Comandos;; .......    
esac     
Exemplos de padrões:    
*.c   *ab   *00*  *ab*  100 alo a*b ab*    
*00*    
1001    
12001    
90003    
1234 NÃO    
    
Case <variável> in    
a)    
echo “a letra digitada foi a”;;    
b)    
echo “a letra digitada foi b”;;    
esac     
    
Comandos para gestão de arquivos e diretórios
Imprime o conteúdo de um arquivo
cat nome do arquivo 

Criar diretório
mkdir nome do diretório

Mostrar o caminho por inteiro do diretório atual    
pwd     
    
Mudar de diretório    
cd nome     
    
Move ou renomeia arquivos ou diretórios    
mv nome    
    
Copiar arquivo    
cp nome arq nome diretório    
    
Remover um diretório    
rmdir nome    
    
Remover um arquivo    
rm nome    




 
