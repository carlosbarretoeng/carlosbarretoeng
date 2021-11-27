# Git & Github

## Semana 1 - Nosso primeiro encontro.!

### Vídeo

[![Watch the video](https://i.ibb.co/xM5p8Mg/Git-Git-Hub-Semana1.png)](https://www.youtube.com/watch?v=7-m8sc-9JDI)
  
### Apresentação

![Apresentacao](https://i.ibb.co/r50kmmy/Git-e-Github-Semana-1.jpg)

[Google Presentation](https://docs.google.com/presentation/d/e/2PACX-1vSl7AJnV3thC_vg1HJzX0SRDgRClt9RBvqR_O9ta_CRgpekPRyjDYs8S64djHwobAvIV447jYtjI4fg/pub?start=false&loop=false)
||
[PDF](https://github.com/carlosbarretoeng/git-e-github/raw/master/Semana1/Git%20e%20Github%20-%20Semana%201.pdf)
  
### CheatSheets

#### Diferenças e Aplicações

* _$ diff_ é usado para localizar as diferenças entre dois arquivos.
* _$ diff -u_ é usado para comparar dois arquivos, linha a linha, e a também apresentar um pouco mais de contexto
```
$ cat menu1.txt
Menu1:

Maças
Bananas
Laranjas
Peras

$ cat menu2.txt
Menu:

Maças
Bananas
Uvas
Morangos

$ diff -u menu1.txt menu2.txt
--- menu1.txt 2021-11-01 18:00:00.000000000 +0300
+++ menu2.txt 2021-11-01 19:00:00.000000000 +0300
@@ -1,6 +1,6 @@
-Menu1:
+Menu:

Maças
Bananas
-Laranjas
-Peras
+Uvas
+Morangos
```

* O comando _patch_ é util para aplicar as mudanças propostas em um 'Arquivo de Diferenças'. Normalmente exportamos o resultado
da execução do comando _diff_ para um arquivo _*.diff_ utilizando o perador de terminal _>_ e depois injetamos esse arquivo na
execução do comando _patch_ utilizando o operador de terminal _<_

```
$ cat hello_world.txt 
Hello World

$ cat hello_world_long.txt 
Hello World

It's a wonderful day!

$ diff -u hello_world.txt hello_world_long.txt 
--- hello_world.txt     2019-12-16 19:24:12.556102821 +0900
+++ hello_world_long.txt        2019-12-16 19:24:38.944207773 +0900
@@ -1 +1,3 @@
 Hello World
+
+It's a wonderful day!

$ diff -u hello_world.txt hello_world_long.txt > hello_world.diff

$ patch < hello_world.diff 
patching file hello_world.txt

$ cat hello_world.txt 
Hello World

It's a wonderful day!
```

### Leituras sugeridas

* Documentação comando _diff_ :: https://man7.org/linux/man-pages/man1/diff.1.html
* Documentação comando _patch_ :: https://man7.org/linux/man-pages/man1/patch.1.html
* Documentação protocolo _GIT_ :: https://git-scm.com/doc
* Definindo seu email no Github :: https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-user-account/managing-email-preferences/setting-your-commit-email-address
