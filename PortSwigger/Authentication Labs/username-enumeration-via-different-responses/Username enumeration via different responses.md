---
attachments: [Clipboard_2026-05-26-23-44-02.png, Clipboard_2026-05-26-23-44-52.png, Clipboard_2026-05-26-23-45-40.png, Clipboard_2026-05-26-23-49-32.png, Clipboard_2026-05-26-23-53-35.png, Clipboard_2026-05-26-23-53-50.png, Clipboard_2026-05-26-23-54-37.png, Clipboard_2026-05-26-23-57-57.png, Clipboard_2026-05-26-23-59-53.png, Clipboard_2026-05-27-00-00-30.png, Clipboard_2026-05-27-00-01-23.png, Clipboard_2026-05-27-00-01-56.png]
title: Username enumeration via different responses
created: '2026-05-27T02:43:20.976Z'
modified: '2026-05-27T03:01:56.060Z'
---

# Username enumeration via different responses

Aqui foi fornecido um dicionario com possiveis usuarios e senhas. Iremos enumerar os usuarios e brute forcar a senha

![](@attachment/Clipboard_2026-05-26-23-44-02.png)

Vamos mandar a requisicao para o intruder

![](@attachment/Clipboard_2026-05-26-23-44-52.png)

E vamos selecionar o ataque sniper, que coloca um valor por vez em um unico campo. Colocaremos na senha uma string grande, que requer mais processamento, evidenciando tempos de resposta

Tambem iremos selecionar os payloads, que serao os lugares onde mudaremos os valores (usuario neste caso). E clicamos em Add.

![](@attachment/Clipboard_2026-05-26-23-53-35.png)

Usaremos simple list, que segue linha por linha para definir os parametros que seráo usados, selecionaremos o campo de usuario em payload position, e clicaremos em load para carregar o dicionario que esta salvo como arquivo texto. 

![](@attachment/Clipboard_2026-05-26-23-53-50.png)

Assim clicamos em Start e comecamos o ataque.

![](@attachment/Clipboard_2026-05-26-23-54-37.png)

Percebemos que nos resultados ha um Lenght diferente, e analisamos

![](@attachment/Clipboard_2026-05-26-23-57-57.png)

Vemos senha incorreta, o que implica que o username esta certo. Vemos o payload usado, colocamos como padrao, e fazemos o mesmo passo para brute forcar a senha.

![](@attachment/Clipboard_2026-05-26-23-59-53.png)

![](@attachment/Clipboard_2026-05-27-00-00-30.png)

Codigo 302! agora e so abrir a requisicao com o navegador e o portswigger contabilizara o lab

![](@attachment/Clipboard_2026-05-27-00-01-23.png)

![](@attachment/Clipboard_2026-05-27-00-01-56.png)


