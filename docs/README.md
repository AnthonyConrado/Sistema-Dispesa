# Sistema de Controle de Despesas

## Objetivo
Desenvolver um sistema simples para **controle de despesas pessoais**, permitindo ao usuário registrar despesas, pagamentos e gerenciar categorias e usuários.  
Todos os dados são armazenados em **arquivos de texto**, garantindo um formato leve e acessível.

---

## Funcionalidades
- **Entrar nova despesa** (descrição, valor, vencimento e categoria)  
- **Anotar pagamento** de uma despesa existente  
- **Listar despesas** pagas ou em aberto (com filtros por período ou categoria)  
- **Gerenciar tipos de despesa** (criar, editar e excluir categorias)  
- **Gerenciar usuários**, com **criptografia de senha** para segurança  

---

## Conceitos de POO Aplicados
- **Classes e Objetos** → modelagem das entidades principais  
- **Herança e Polimorfismo** → especialização de tipos de despesa  
- **Interfaces** → definição de contratos para classes pagáveis  
- **Sobrecarga de Construtores** → flexibilidade na criação de objetos  
- **Métodos e Atributos Estáticos** → controle global de contadores  
- **Criptografia Simples** → proteção das senhas de usuários
