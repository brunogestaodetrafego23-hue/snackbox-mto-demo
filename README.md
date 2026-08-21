# SnackBox MTO — demonstração pública

Aplicação web responsiva para gestão interna de uma snackbox: produtos, stock, consumos, pagamentos, caixa e lista de compras.

## Demonstração

Esta versão pública funciona integralmente no navegador, com dados fictícios e sem ligação ao sistema real.

- PIN de demonstração: `1234`
- Não recolhe nem envia dados
- Não escreve em Google Sheets
- Não contém tokens, credenciais ou URLs privadas
- Os dados são repostos ao recarregar a página

## Funcionalidades demonstradas

- Registo de consumos por utilizador
- Gestão de produtos, preços e stock
- Lista de compras e confirmação de reposição
- Pagamentos e controlo de caixa
- Área de administração
- Interface adaptada a telemóvel e desktop

## Arquitectura do protótipo original

O protótipo privado usa:

- HTML, CSS e JavaScript numa aplicação de página única
- Google Apps Script como API
- Google Sheets como armazenamento
- GitHub para controlo de versões e alojamento da demonstração

A arquitectura com Apps Script e Sheets foi adequada para validar rapidamente o fluxo e a experiência com baixo custo. Não é apresentada como substituto de um backend com autenticação, autorização por utilizador, base de dados e políticas de acesso, como Supabase, para dados sensíveis ou produção em escala.

## Separação de segurança

O frontend público deste repositório está em modo `DEMO_MODE` e usa apenas um armazenamento temporário em memória. A API, a folha de cálculo, os identificadores de implementação e os segredos do protótipo privado não fazem parte da demonstração.

> Um token colocado no JavaScript do navegador nunca é secreto. Por isso, a versão pública não inclui qualquer token nem endpoint do Apps Script.

## Estado

Projecto de portefólio / prova de conceito. Os dados, nomes e movimentos apresentados são fictícios.
