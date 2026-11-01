<h1 align="center">Sistema de Controle de Despesas</h1>

<p align="center">
  Aplicação de console em <strong>Java</strong> para organizar despesas pessoais, criada para praticar <strong>Programação Orientada a Objetos</strong>.
</p>

<p align="center">
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white">
  <img alt="POO" src="https://img.shields.io/badge/POO-orienta%C3%A7%C3%A3o%20a%20objetos-b794f6?style=for-the-badge">
  <img alt="Versão v0.0.3" src="https://img.shields.io/badge/vers%C3%A3o-v0.0.3-6d3fd6?style=for-the-badge">
</p>

---

## Sobre o projeto

Sistema simples para controle de despesas pessoais, com cadastro de despesas, pagamentos, tipos de despesa e usuários. O foco do projeto é aplicar os conceitos de POO em um problema do dia a dia: cada parte do domínio virou uma classe com responsabilidade própria.

A documentação original, com o histórico de versões, está em [`docs/README.md`](docs/README.md).

## Funcionalidades

O menu principal oferece:

```
==== SISTEMA DE CONTROLE DE DESPESAS ====
1 - Entrar Despesa
2 - Anotar Pagamento
3 - Listar Despesas em Aberto
4 - Listar Despesas Pagas
5 - Gerenciar Tipos de Despesa
6 - Gerenciar Usuários
0 - Sair
```

E as classes do domínio:

| Classe | Responsabilidade |
| --- | --- |
| `Despesa` | Descrição, valor, vencimento, categoria e situação (paga ou em aberto) |
| `TipoDespesa` | Categorias usadas para classificar as despesas |
| `Usuario` | Nome, login e senha guardada de forma cifrada, com validação de senha |
| `Main` | Menu interativo no terminal |

## Conceitos de POO aplicados

- Classes e objetos
- Encapsulamento (atributos privados e métodos de acesso)
- Construtores com regras de inicialização (toda despesa começa "em aberto")
- Sobrescrita de `toString()` para exibição dos dados
- Método privado para cifrar a senha, que nunca fica guardada em texto puro

## Como rodar

Pré-requisito: [JDK](https://adoptium.net/) 11 ou superior.

```bash
git clone https://github.com/AnthonyConrado/Sistema-Dispesa.git
cd Sistema-Dispesa

javac -d out src/*.java
java -cp out Main
```

## Estrutura

```
Sistema-Dispesa/
├── src/
│   ├── Main.java          # menu principal
│   ├── Despesa.java
│   ├── TipoDespesa.java
│   └── usuario.java       # classe Usuario
└── docs/
    └── README.md          # documentação e changelog
```

## Versões

| Versão | O que mudou |
| --- | --- |
| v0.0.1 | Criação do menu principal com as opções básicas |
| v0.0.2 | Separação das classes e definição do MVP |
| v0.0.3 | MVP completo, README documentado e tag de versão |

## Próximos passos

- [ ] Renomear `usuario.java` para `Usuario.java` (o Java exige que o arquivo tenha o nome da classe pública)
- [ ] Ligar cada opção do menu às classes do domínio
- [ ] Salvar despesas e usuários em arquivo de texto
- [ ] Trocar o hash da senha por um algoritmo seguro (SHA-256 com salt)

## Autor

Feito por **Anthony Gonçalves Conrado**, desenvolvedor full stack júnior em Guarulhos, SP.

[![GitHub](https://img.shields.io/badge/GitHub-AnthonyConrado-181717?style=flat-square&logo=github)](https://github.com/AnthonyConrado)
[![E-mail](https://img.shields.io/badge/E--mail-anthonyns973%40icloud.com-b794f6?style=flat-square&logo=maildotru&logoColor=white)](mailto:anthonyns973@icloud.com)
