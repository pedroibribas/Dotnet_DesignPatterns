## DesignPatterns
Projeto DotNet que reúne cases de padrões de design para estudo e prática.
Sua estrutura é:
```bash
|-- DesignPatterns.Console # programa para rodar a aplicação
|-- DesignPatterns.Core    # bibliotecas com cases de padrões 
|-- DesignPatterns.Utils
```

## Rodando a aplicação *[em construção]*

## Conceitos *[em construção]*
- Padrões de Projetos (Design Patterns): Os padrões de projeto - design patterns - são alternativas para que o desenvolvedor consiga escrever código com responsabilidades mais bem definidas, com um baixo acoplamento, e que evolua de maneira natural. Características essas que não são encontrados em sistemas procedurais, que tipicamente apresentam código complexo, cheio de ifs, e que fazem muita coisa, tornando a manutenção custosa. Códigos que fazem bom uso de OO evoluem geralmente não pela adição de mais um if, mas sim pela criação de mais uma estratégia, mais um observador, mais um estado, e assim por diante. Padrões de projeto no fim apenas fazem bom uso da orientação a objetos, e seus conceitos e mecanismos, como encapsulamento, abstrações, interfaces, polimorfismo, e etc. Não. Padrões de projeto trazem grande flexibilidade ao seu código, mas isso tem um preço: complexidade. Naturalmente um código que faz uso de padrões de projeto é, do ponto de vista de implementação, mais complexo do que um código que não os utiliza. Afinal, como tudo está desacoplado, o desenvolvedor precisa entender melhor a solução para entender o que o código faz como um todo. Um bom desenvolvedor sabe fazer essa avaliação e entender quais os ganhos e perdas da utilização de um padrão. Em um problema simples de resolver, talvez o uso de um padrão de projeto não faça sentido; o código vai apenas ficar mais complicado. Agora, em problemas que são por natureza complexos, ou que demandam flexibilidade, pois mudam o tempo todo, talvez a utilização de um padrão de projeto traga benefícios, já que todos os padrões sempre agregam flexibilidade ao código gerado. Nunca se esqueça: a sua experiência é fundamental! Padrões de projeto são mais uma ferramenta. Eles devem ser um meio para se chegar à solução final, e não o "fim", ou seja, o seu objetivo principal.
- Estratégia
/**
* Os padrões de projeto resolvem problemas como:
* - diminui o tamanho do código
* - reduz complexidade do código
* - reduz uso de diversas variáveis, ifs e fors no mesmo método
* - reduz demora para compreender o que um método faz ou onde está o código que faz uma alteração
* - reduz classes alteráveis em uma manutenção 
*/

// Exemplo Investiment.cs
// Resumo: é feito um investimento financeiro a partir de 
// um saldo bancário, conforme o nível de agressividade
// do investidor, e é retornado o saldo resultante.
    /**
        * Agora temos um método independente de um imposto concreto, e que depende apenas
        * da abstração ITax, de modo genérico. As classes concretas de impostos se tornam
        * estratégias do ITax.
        * 
        * O uso de estratégias a partir de uma abstração é o padrão de projeto Strategy.
        */

            /**
     * Cada imposto concreto é uma estratégia do contrato ITax.
     * O sistema aproveitará apenas a abstração.
     * 
     * Cada regra de imposto em concreto é ENCAPSULADO em uma classe especializada 
     * e coesa (responsabilidade única).
     * 
     * O padrão Strategy facilita a geração de novas estratégias, por meio do
     * polimorfismo, sem provocar uma manutenção sistêmica.
     */