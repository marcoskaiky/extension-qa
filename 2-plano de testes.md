# Plano de Testes — SIFIT

> 🔲 **Status: ainda não iniciado.** Modelo de plano de testes, a ser preenchido conforme a execução avançar.

## 1. Objetivo

Definir o escopo, a estratégia e os critérios utilizados para testar manualmente as funcionalidades do sistema SIFIT, como parte do trabalho de extensão de Qualidade de Software.

## 2. Escopo

Serão testadas as funcionalidades listadas em [`1-Analise de requisitos.md`](./1-Analise%20de%20requisitos.md): Autenticação, Pessoas/Alunos, Planos, Anamnese, Pontuação, Produtos/Pedidos, Posts e Permissões.

Fora do escopo: testes de performance/carga, testes de segurança aprofundados (pentest), testes automatizados.

## 3. Ambiente de testes

| Item | Valor |
|---|---|
| URL do sistema | `https://sifit.centrion.com.br` |
| Usuário de teste | fornecido pelo professor (não publicar no repositório) |
| Banco de dados | MySQL — host `srv795.hstgr.io`, porta `3306`, schema `u339572246_alfa1` (acesso somente para consulta/validação, não publicar credenciais) |
| Navegador | Google Chrome (última versão estável) |
| Ferramenta de evidência em vídeo | Extensão **Jam** |

> ⚠️ Não inclua usuário/senha reais neste arquivo nem em prints. Use `********` ou edite a imagem antes de subir ao GitHub.

## 4. Estratégia de testes

- **Testes Funcionais:** validar se cada funcionalidade faz o que deveria.
- **Testes Positivos:** usar dados válidos e fluxos esperados.
- **Testes Negativos:** usar dados inválidos, campos vazios, formatos incorretos.
- **Testes Exploratórios:** navegação livre buscando comportamentos inesperados.
- **Validação em banco de dados:** conferir, via MySQL Workbench, se a ação feita na tela realmente refletiu na tabela correspondente.

## 5. Técnicas e formatos

- Casos de teste em formato **BDD (Gherkin)** — `Dado / Quando / Então` — na pasta [`Cenarios de testes/`](./Cenarios%20de%20testes/).
- Checklist de execução por funcionalidade.
- Evidências: prints de tela (passo a passo) + vídeo gravado com a extensão Jam, armazenados no Google Drive e referenciados nos relatórios.

## 6. Cronograma

| Etapa | Status |
|---|---|
| Análise de requisitos | ⬜ Pendente / ✅ Concluído |
| Elaboração dos cenários de teste | ⬜ Pendente / ✅ Concluído |
| Execução dos testes | ⬜ Pendente / ✅ Concluído |
| Registro de bugs | ⬜ Pendente / ✅ Concluído |
| Relatório final | ⬜ Pendente / ✅ Concluído |

## 7. Critérios de entrada e saída

**Entrada:** acesso liberado ao sistema SIFIT e ao banco de dados; análise de requisitos concluída.

**Saída:** todos os cenários planejados executados, bugs encontrados documentados em [`3-Relatorio-de-Bugs.md`](./3-Relatorio-de-Bugs.md) e resultado consolidado em [`4-Relatorio dos testes.md`](./4-Relatorio%20dos%20testes.md).
