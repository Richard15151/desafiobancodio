# Desafio: Modelando um Sistema Bancário com POO em Python

Este projeto é a solução para o desafio "Modelando um Sistema Bancário com POO" do bootcamp de Python da [DIO (Digital Innovation One)](https://www.dio.me/). O objetivo foi refatorar um sistema bancário simples, originalmente procedural, aplicando os conceitos fundamentais da Programação Orientada a Objetos para criar um código mais modular, reutilizável e organizado.

## 🚀 Funcionalidades

O sistema é controlado por um menu interativo no terminal e oferece as seguintes operações:

- **Criar Cliente (Usuário):** Cadastra um novo cliente (Pessoa Física).
- **Criar Conta Corrente:** Associa uma nova conta a um cliente existente.
- **Depositar:** Realiza depósitos em uma conta.
- **Sacar:** Realiza saques, respeitando um limite por saque e um número máximo de saques diários.
- **Exibir Extrato:** Mostra o histórico de transações e o saldo atual da conta.
- **Listar Contas:** Exibe todas as contas correntes cadastradas no sistema.

## 🛠️ Conceitos de POO Aplicados

A estrutura do projeto foi pensada para aplicar os pilares da POO:

- **Abstração:** Classes como `Conta` e `Transacao` definem a base para tipos mais específicos.
- **Encapsulamento:** Atributos privados (`_saldo`, `_agencia`) são acessados de forma controlada através de propriedades (`@property`).
- **Herança:** As classes `PessoaFisica` herdam de `Cliente`, e `ContaCorrente` herda de `Conta`, reutilizando e estendendo funcionalidades.
- **Polimorfismo:** O método `sacar` é sobrescrito em `ContaCorrente` para adicionar regras de negócio específicas, e o método `registrar` é implementado de maneiras distintas nas classes `Saque` e `Deposito`.

## ⚙️ Como Executar

1. Certifique-se de ter o Python 3 instalado em sua máquina.
2. Clone ou faça o download deste repositório.
3. Navegue até o diretório do projeto pelo terminal.
4. Execute o script `app.py`:

```bash
python app.py
```
5. Siga as instruções apresentadas no menu interativo para utilizar o sistema.