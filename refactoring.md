Refactoring
===


######  by Wagner Rodrigues ( [@vavaRodrigues](https://github.com/vavaRodrigues) )

---

# Talking about

- **Refactoring: Third stage of Test-Driven Development (Red, Green, Refactor)**
- **Refactoring an existing production code**

---

# Vamos falar apenas do segundo item.

A necessidade de uma refatoração dá-se inicialmente por uma decisão de um ou mais programadores sob um determinado trecho de código, por concluir de que aquilo não está construído de uma maneira aceitável.


---


# Martin Fowler disse:

"Refatorar quer dizer, não mudar o comportamento da parte a ser substituída."

Apesar de óbvio, essa primeira premissa é a mais violada ao refatorar algo, pois junto da refatoração o programador resolve fazer umas coisinhas a mais para aproveitar já que ele esta refatorando.


---


# Mas porque isso não funcina bem?


---


Ao refatorar você pode quebrar coisas. E, para evitar que essa quebra não vá parar em produção, você precisa de respostas rápidas à quaisquer mudanças que faça no código, por menores que sejam. Ai é quando dizemos (Welcome, Test-First).


---


Devemos evitar com todas as nossas forças ficar criando tarefas de refatoração no projeto. **A refatoração deve vir com um propósito.** Prever o futuro não é um propósito. **Não há necessidade de refatorar algo que está em produção há tempos só pelo prazer de refatorar um trecho de código.** (essa parte podemos deixar para fazer em casa :wink: ), pois você já deveria ter feito isto no terceiro passo do TDD: (Red, Green, **Refactor**).


---


# O ponto é :

Se não o fez, espere até que venha precisar trabalhar com aquele código novamente para implementar uma nova feature, daí, divida essa feature em duas etapas: refatorar o código envolvido na nova tarefa e fazer a nova tarefa.


---



 Sempre ao pegar um código é um costume a gente não entender o que aquilo faz e por que faz. Por não entender, a gente vai e diz: ah, isso aqui precisa de uma refatoração. Será mesmo?

Esse tipo de atitude pode colocar em xeque os benefícios da refatoração e pior: quebrar algo em produção desnecessariamente, pura e simplesmente porque você sendo novo naquele projeto/equipe não entendeu o código – o que é normal em todo início. Com isso, você faz feio com a equipe e pode destruir todo um processo de amostragem e explicação sobre benefícios de uma refatoração planejada.

É importante que você vá com calma e espere até ter uma certeza mais clara das coisas.


---

# O que eu vou falar pode impactar... 

## REFATORAÇÃO NEM SEMPRE É A MELHOR SAÍDA 

---


Outro ponto a favor de evitar sair refatorando sem saber quem nem porquê é ter o controle analítico de analisar o cenário em questão e verificar se a refatoração de código solucionaria o problema. Já vi casos em que o código em si não estava ruim. O verdadeiro problema era um design mal pensando e neste caso, a refatoração não ajudaria em nada. Você precisaria ir além nas decisões.

É preferível manter um código espaguete por mais um tempo do que perder a talvez única chance de mostrar os benefícios.


---


# Resumo do que falamos...

---
- Respostas rápidas ao refatorar. Teste de unidade é a única forma de conseguir isto rapida e isoladamente;
---

- Refatorar. Depois de pronto, volte para implementar o que ia fazer no começo. Não faça os dois juntos por mais que Goku desça da núvem para te pedir isto;

---
- Refatorar ao entrar num projeto:  ![](images/its-a-trap.jpeg)

---
- Às vezes é melhor um git reset mental e partir para outra solução;

```html
$ git reset 
```


---
- Estar apoiado em teste de unidade e test-first trará a confiança necessária para tomar a decisão de refatorar;
---
- Esforce-se para não tornar a refatoração uma task do seu projeto. Ela deve ser junto de uma task de -implementação. Refatorar precisa de propósito, e;
---
- Red, Green, **Refactor** (TDD) != Refatorar código de produção.
---

# Recomended books

* Refactoring: Improving the Design of Existing Code

# Online courses

Refactoring


* https://sourcemaking.com/refactoring




