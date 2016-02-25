
.
![](vim.png)
# Vim as a Python IDE


# Why Vim?

- É ubíquo, encontrado em toda instalação Linux e Mac OSX
- É altamente customizável
- Extremamente leve e poderoso, abre arquivos de centenas de Mbytes
- Pode ser usado para editar qualquer linguagem
- É viciante

# Why not?

- Curva de aprendizado lenta
- Difícil lembrar todos os comandos possíveis
- Primeira experiência normalmente é frustrante


# Learning

Aprendizado interativo disponível junto com a instalação do Vim

- Vimtutor


# Modal Editing

Dependendo do modo, as teclas servem para coisas diferentes

- Normal mode (ESC)
- Insert mode (i)
- Visual mode (v)
- Ex mode


# Normal mode

:w salva
:q sai 
:q! sai sem salvar


# Moving

   <-h j k l->

Desabilite as setas


# Move faster

- ^e - move a janela para baixo
^y - move a janela para cima
^f - move uma página para baixo
^b - move uma página para cima

- H - move cursor para o topo da janela
M - move cursor para o meio da janela
L - move cursor para o final da janela

- gg - início do arquivo
G - final do arquivo


# Search

/{texto} - busca o texto adiante no arquivo
?{texto} - busca o texto para trás no arquivo
n - encontra a próxima ocorrência

# Change

:%s/old/new/gc


# Comandos

d - delete (cut)
c - change (apaga e coloca no modo de inserção)
y - yank (copy, ctl-c)
p - paste  (ctl-v)
v - visually select
 

# Text objects

w - (w)ords
s - (s)entences
p - (p)aragraphs


# Motions

a - all
i - in
t - 'til
f - find forward
F - find backward


# Combine everything

{command}{text object or motion}

diw
delete in word

caw
change all word

yi)
yank all text inside parentheses


# More commands

dd / yy - delete/yank a linha atual
D / C - delete/change até o final da linha
^ / $ - move para o início/final da linha
I / A - move para início/final da linha e coloca no modo de inserção
o / O - insere nova linha acima/abaixo da linha corrente e insere


# Repeating

. Dot command


# Macros

Salve comandos em um registrador para repetições

q{registrador}
....  comandos ....
q

@registrador


# Turbinando com Plugins

-Neobundle
-Gundo
-Vim-airline
-Easymotion
-Python-mode
-Syntastic
-Neocomplete
