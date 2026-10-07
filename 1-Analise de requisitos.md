# Análise de Requisitos — SIFIT

> 🔲 **Status: ainda não iniciado.** Este documento é só o esqueleto — nenhuma tela foi explorada/confirmada ainda. Preencher depois de acessar o sistema.

## 1. Sobre o sistema

O **SIFIT** (`sifit.centrion.com.br`) é um sistema de gestão para academias/estúdios de treino, contemplando cadastro de alunos, planos, anamnese, pontuação/gamificação, produtos e pedidos.

> Preencha/ajuste esta seção depois de navegar pelo sistema logado, confirmando o propósito de cada módulo.

## 2. Escopo da análise

Este documento mapeia as funcionalidades do sistema que serão cobertas pelos testes manuais deste repositório. Baseado na navegação pela tela e na estrutura do banco de dados (schema `u339572246_alfa1`), os principais módulos identificados são:

| Módulo | Descrição | Tabelas relacionadas (referência) |
|---|---|---|
| Autenticação | Login/logout de usuários do sistema | — |
| Pessoas / Alunos | Cadastro e gestão de pessoas e alunos | `pessoas`, `pr_alunos` |
| Planos | Planos de academia e vínculo com clientes | `planos`, `plano_clientes`, `plano_sifit` |
| Anamnese | Perguntas e respostas de ficha de anamnese | `perguntas_anamnese`, `pergunta_ficha` |
| Pontuação / Gamificação | Pontuação de clientes por pedidos e produtos | `pontuacao`, `pontuacao_pedido`, `pontuacao_produto` |
| Produtos e Pedidos | Catálogo de produtos e pedidos realizados | `produtos`, `pedidos` |
| Posts / Marcações | Postagens e marcações (feed social) | `posts`, `posts_marcacoes` |
| Permissões | Controle de acesso por função | `permissoes`, `permissao_funcao` |

> ⚠️ Ajuste esta tabela conforme você explorar o sistema — nem toda tabela do banco corresponde a uma tela visível, e pode haver telas sem tabela óbvia.

## 3. Requisitos funcionais (RF)

Preencha conforme for confirmando o comportamento esperado de cada tela, por exemplo:

| ID | Requisito | Descrição |
|---|---|---|
| RF-01 | Login | O sistema deve permitir login com usuário e senha válidos |
| RF-02 | Cadastro de aluno | O sistema deve permitir cadastrar uma nova pessoa/aluno |
| RF-03 | Cadastro de plano | O sistema deve permitir associar um plano a um cliente |
| RF-04 | Anamnese | O sistema deve permitir preencher/consultar a ficha de anamnese de um aluno |
| RF-05 | Pontuação | O sistema deve calcular/exibir a pontuação do cliente a partir de pedidos/produtos |
| RF-06 | Produtos e pedidos | O sistema deve permitir cadastrar produtos e registrar pedidos |
| RF-07 | ... | ... |

## 4. Requisitos não funcionais (RNF)

| ID | Requisito | Descrição |
|---|---|---|
| RNF-01 | Usabilidade | Telas devem ser claras e sem erros de navegação |
| RNF-02 | Desempenho | Telas devem carregar em tempo aceitável |
| RNF-03 | Segurança | Dados sensíveis (senha, CPF) não devem ficar expostos em tela ou log |

## 5. Observações / dúvidas levantadas

- (liste aqui pontos que precisam de confirmação com o professor/sistema)
