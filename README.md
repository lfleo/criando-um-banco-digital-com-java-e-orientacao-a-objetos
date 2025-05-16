# Criando um Banco Digital com Java e Orientação a Objetos

Projeto desenvolvido com foco em aplicar os principais conceitos da **Programação Orientada a Objetos (POO)** em Java, como **abstração**, **encapsulamento**, **herança** e **polimorfismo**.

## 🧠 Cenário do Desafio

> "Um banco oferece aos seus clientes dois tipos de contas (Corrente e Poupança), as quais possuem as funcionalidades de **depósito**, **saque** e **transferência** (entre contas da própria instituição)."

---

## 🎯 Objetivo

Modelar uma estrutura orientada a objetos para simular o funcionamento básico de um banco digital, onde o foco está na correta aplicação dos pilares da POO, abstraindo os detalhes técnicos e enfatizando a estrutura conceitual.

---

## 🧱 Conceitos Aplicados

### 🔹 Abstração
A abstração permite representar entidades do domínio bancário com objetos no código. Neste projeto, representamos contas bancárias e clientes por meio de classes, focando apenas nos comportamentos e atributos essenciais.

- Exemplo: `Conta`, `Cliente`, `Banco`

### 🔹 Encapsulamento
Escondemos os detalhes internos de implementação das classes, expondo apenas o necessário por meio de métodos públicos (`getters`, `setters`, `depositar()`, `sacar()`, `transferir()`), tornando o código mais seguro e modular.

- Benefícios: Manutenção facilitada e maior segurança na manipulação de dados.

### 🔹 Herança
Criamos uma estrutura onde `ContaCorrente` e `ContaPoupanca` **herdam** da classe abstrata `Conta`, aproveitando código comum e permitindo especializações por tipo de conta.

- Exemplo:
  ```java
  public abstract class Conta {
      // código comum a todas as contas
  }

  public class ContaCorrente extends Conta {
      // comportamentos específicos da conta corrente
  }

  public class ContaPoupanca extends Conta {
      // comportamentos específicos da conta poupança
  }
