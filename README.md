🏅 Sistema de Gerenciamento de Atletas
📋 Sobre o Projeto
Esta aplicação JavaScript orientada a objetos foi desenvolvida para gerenciar informações de atletas em competições esportivas. O sistema calcula automaticamente categoria, IMC e média válida das notas, seguindo regras específicas da competição.

🎯 Objetivo
Criar uma classe Atleta capaz de armazenar informações pessoais e notas de atletas, além de calcular automaticamente parâmetros importantes para avaliação esportiva.

⚙️ Funcionalidades
✅ Armazena dados completos do atleta (nome, idade, peso, altura, notas)

✅ Calcula categoria baseada na idade

✅ Calcula IMC (Índice de Massa Corporal)

✅ Calcula média válida desconsiderando maior e menor nota

✅ Métodos getters para acesso organizado aos dados

✅ Exibição formatada de todos os dados

🏗️ Especificações Técnicas
📊 Estrutura da Classe Atleta
Atributos:

nome - Nome completo do atleta

idade - Idade em anos

peso - Peso em kg

altura - Altura em metros

notas - Array com 5 notas

Métodos Principais:

calculaCategoria() - Define categoria por idade

calculaIMC() - Calcula Índice de Massa Corporal

calculaMediaValida() - Calcula média das 3 notas centrais

Métodos Getters:

obtemNomeAtleta(), obtemIdadeAtleta(), obtemPesoAtleta()

obtemAlturaAtleta(), obtemNotasAtleta()

obtemCategoria(), obtemIMC(), obtemMediaValida()

📐 Regras de Cálculo
🎯 Categorias por Idade:
Infantil: 9 a 11 anos
Juvenil: 12 e 13 anos
Intermediário: 14 e 15 anos
Adulto: 16 a 30 anos
Sem categoria: demais idades

⚖️ Cálculo do IMC:
IMC = peso / (altura × altura)

📊 Média Válida
Ordena as 5 notas em ordem crescente
Descarta a maior e a menor nota
Calcula média das demais notas

💡 Tecnologias e Conceitos Utilizados
JavaScript ES6+

Programação Orientada a Objetos

Métodos de Array: sort(), slice(), reduce(), join()

Template Strings para formatação

Encapsulamento com métodos getters

🎯 Exemplo de Processamento
Para o atleta de exemplo:

Notas originais: [10, 9.34, 8.42, 10, 7.88]

Notas ordenadas: [7.88, 8.42, 9.34, 10, 10]

Notas válidas: [8.42, 9.34, 10]

Média: (8.42 + 9.34 + 10) ÷ 3 = 9.2533...

Categoria: 30 anos → "Adulto"

IMC: 80 ÷ (1.70 × 1.70) = 27.68

Exemplo de Implementação
criando um atleta
const atleta = new Atleta(
"Cesar Abascal",
30,
80,
1.70,
[10, 9.34, 8.42, 10, 7.88]
);

// Exibindo dados completos
console.log(atleta.exibirDadosCompletos());

Saida Esperada:
Nome: Cesar Abascal
Idade: 30
Peso: 80 kg
Altura: 1.7 m
Notas: 10, 9.34, 8.42, 10, 7.88
Categoria: Adulto
IMC: 27.68
Média Válida: 9.25

👨‍💻 Desenvolvido para:

Sistema desenvolvido para organização de competições esportivas, demonstrando aplicação prática de programação orientada a objetos em JavaScript para solução de problemas reais.

Este projeto implementa um sistema completo de gerenciamento de atletas, aplicando conceitos avançados de JavaScript e boas práticas de desenvolvimento.
