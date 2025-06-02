# ***Explicação do jogo do número secreto***
```js
alert('Boas vindas ao jogo do numero secreto!');
let numeroMaximo = 50;
let numeroSecreto = parseInt(Math.random() * numeroMaximo + 1);
console.log(numeroSecreto);
let chute;
let tentativas = 1;

//enquanto o chute nao for igual ao nmumro secreto
while (chute != numeroSecreto) {
    chute = prompt(`Escolha um numero entre 1 e ${numeroMaximo} `);
    // se o chute for igual ao numero secreto
    if (chute == numeroSecreto) {
        break;
    } else {
        if (chute > numeroSecreto) {
            alert(`O número secreto é menor que o ${chute}`);
        } else {
            alert(`O número é maior que o ${chute}`);
        }
        //tentativas = tentativas + 1;
        tentativas++;
    } 
}
let palavraTentativa = tentativas > 1 ? 'tentativas' : 'tentativa';
alert(`Isso ai! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativa}`);
```
Bom, nesse exercício/aula, foi dado para fazermos um jogo básico, que o intuito é descobrir o número secreto. Nesse curso, aprendemos a usar o ternário, que nada mais é do que um if-else menor, sem ter repetições (nessas últimas atividades teve um bem didático).

Outra coisa importante é o pseudo gerador de números aleatórios, que basicamente vai funcionar daquela forma que está dito no código. Coloquei uma variável única (`numeroMaximo`), para não ter que ficar mexendo em várias outras coisas toda hora que for mudar o número máximo do jogo. Assim, basta eu apenas mudar o valor daquela variável que todos os outros mudam automaticamente.

Também vimos sinais novos, como o `!=`, `++` e o `break`, que, pra ser sincero, eu não sei o que fazem — vou deixar o pesquisar e falar o que eles fazem.
\[**Comentário:**

* `!=` significa "diferente de"; ele verifica se dois valores **não são iguais**.
* `++` serve para **incrementar** (aumentar) uma variável em 1, tipo: `contador++` é o mesmo que `contador = contador + 1`.
* `break` é usado para **sair de um loop** ou estrutura antes que ela termine naturalmente.]

Usei muito template string, acho que é uma prática boa a ser usada. Ela é bem útil e deixa o código bem rico.

Entretanto, eu acho que é isso.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
