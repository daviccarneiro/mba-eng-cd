---
date: 2026-04-25
title: Database Modeling
prof: Vladimir
---
---

**Tipos de modelos de dados**
- Conceitual
- Lógico
- Físico

---

- Mini mundo
	- O que eu desejo mapear num banco de dados
- Modelo descritivo

- Levantamento de Requisitos

---
## Modelo Entidade Relacionamento (MER)
- Desenvolvido por Peter Chen

Mapear o banco de dados baseado em:
- Entidades
- Relacionamentos

Retangulo → Entidade
- Persona, algo do mundo real
- Pessoa (fisica,juridica) ou processo
- Proceso (cliente, usuario, venda)
- e.g. Aluno

Losangos → Relações
- Geralmente dão verbos
- Relações entre entidades
- e.g. Cliente **realiza** compra

Relacionamentos são bidirecionais

Funcionario → Trabalha → Projeto
OU
Projeto → Trabalha → Funcionário


Cardinalidade → (1,n)
- 1 → cardinalidade mínima
- n → cardinalidade máxima

Relacionamento Binário
![[Pasted image 20260425113052.png|411]]

Relacionamento Ternário
![[Pasted image 20260425113130.png|380]]

Atributos
- Toda entidade tem que ter pelo menos um atributo

Tipos de Atributos
- Bola vazia: preenchiemnto opcional
- Bola cheia: obrigatório
(DEPENDE DA NOTAÇÃO)

Atributo derivado → Calculado por um atributo anterior
![[Pasted image 20260425113656.png]]

Tefone com duas bolinhas → Multivalorado, pode ter mais de um

Auto-relacionamento
![[Pasted image 20260425130812.png|464]]

Um funcionario gerencia outros

Generalização x Especialização
![[Pasted image 20260425131122.png]]



---
T = Conteúdo Total
- Toda instância de um elemento "E" deve pertencer também a uma instancia em uma entidade filha especializada
P = Conteúdo pARCIAL
- Pode existir uma instancia 

E = Cobertuda Exclusiva

S = Cobertura 

## Agregação
![[Pasted image 20260425132646.png]]
Perceba: Relacionamento (GERA) se relacionado com o agregado.

### Referência circular
- Geralmente indica um erro

---

## CONCEITUAL → LÓGICO

Entidade = TABELA

## Chave primárioa
- Valor único
- Preferencialemnte inteiro
- Não nulo
- Sequencial e crescente
- Não multavel

