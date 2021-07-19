# Bateria_com_JavaScript
### Evento 7 projetos com JavaScript da B7WEB

Primeiro projeto da Semana 7 projetos com JavaScript 
Criamos uma bateria no Browser usando JavaScript puro, HTML e CSS.  
Ao precionar as teclas (q,w, e, a, s, d, z, x, c, " "), reproduzimos arquvios de som que estão dentro do projeto.
Também podemos escrever uma sequencia dos caracteres informados a cima em um input, ao precionar o botão o programa reprodus as batidas  
de manereira a imitar uma bateria.


A unica alteração que fiz no projeto foi, adicionar a função:
~~~javascript
function isSongKey(evt){
	var charCode = (evt.which) ? evt.which : evt.keyCode;
    //Valor ascii das teclas de musica
    let keysAccepted = [81, 87, 69, 65, 83, 68, 90, 88, 67, 32];
    return keysAccepted.includes(charCode) ? true : false;
}
~~~
Sem essa função, o campo input recebia qualquer valor digitado, causando um atrasso no som emitido.


