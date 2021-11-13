# Git & Github

## Semana 1

### Vídeo

[![Watch the video](https://i.ibb.co/xM5p8Mg/Git-Git-Hub-Semana1.png)](https://vimeo.com/640753215/ab7ec0e700)
  
### Apresentação

[![Apresentacao](https://i.ibb.co/r50kmmy/Git-e-Github-Semana-1.jpg)](https://docs.google.com/presentation/d/e/2PACX-1vSl7AJnV3thC_vg1HJzX0SRDgRClt9RBvqR_O9ta_CRgpekPRyjDYs8S64djHwobAvIV447jYtjI4fg/pub?start=false&loop=false&delayms=3000)
  
### Resumo
  
| Comando | Exemplo | Descrição |
|------|------|------|
| $ cat [ARQUIVO] | $ cat index.html | O comando _cat_ imprime no terminal o arquivo |
| $ diff [ARQUIVO A] [ARQUIVO B] | $ diff index.html novo_index.html | Exibe a diferença entre o _ARQUIVO A_ e o _ARQUIVO B_ |
| $ diff -u [ARQUIVO A] [ARQUIVO B] | $ diff -u  index.html novo_index.html | Exibe a diferença entre o _ARQUIVO A_ e o _ARQUIVO B_ adicionando um pouco mais de contexto à diferença|
| $ diff -u [ARQUIVO A] [ARQUIVO B] > [ARQUIVO DIFF] | $ diff -u index.html novo_index.html > mudancas.diff | O uso do sinal _>_ faz com que a saída do comando seja salva em um arquivo textual. No exemplo o 'mudancas.diff' |
| $ patch [ARQUIVO A] < [ARQUIVO DIFF] | $ patch index.html < mudancas.diff | O comando patch vai aplicar no _ARQUIVO A_ as mudanças vindas do _ARQUIVO DIFF_ geradas anteriormente |
|------|------|------|
| $ git --version | | Apresenta a versão do comando git instalada na sua máquina |
| $ git config ![--global] user.[email ou name] "..." | $ git config --global user.email "joao@da.silva" | Define as configurações do protocolo git. A flag '--global', que é opcional, faz essa definição para toda a máquina. Sem ela, a configuração fica restrita a um repositótio. |
| $ git init | | Inicializa um repositório local |
| $ git add [. ou * ou ARQUIVO] | $ git add index.html | Envia um determinado arquivo para a _staging area_, fazendo com que as mudanças sejam rastreadas. Os caracteres de ponto (.) ou asterísco (\*) são coringas para adicionar todos os arquivos recentemente modificados na _staging area_ |
| $ git status | | Exibe detalhadamente a situação atual dos arquivos no repositório |
| $ git commit | | Abre o editor padrão para que você possa descrever a mensagem de envio das mudanças da _staging area_ para o repositório |
| $ git commit -m "..." | | Versão simplificada do comando acima. Você pode enviar uma mensagem curta para o commit |
| $ git log | | Exibe o histórico de mudanças rastreadas no repositório |




