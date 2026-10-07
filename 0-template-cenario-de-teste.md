# Template — Cenário de Teste

> Copie este arquivo para cada funcionalidade testada (ex.: `1-login.md`, `2-cadastro-aluno.md`, `3-planos.md`...) e preencha os campos abaixo.

## Funcionalidade: (nome da funcionalidade)

**Tipo de teste:** Funcional / Positivo / Negativo / Exploratório

**Requisito relacionado:** RF-0X (ver `1-Analise de requisitos.md`)

---

### Cenário 1: (descrição curta do caminho feliz)

```gherkin
Dado que o usuário está na tela de login do SIFIT
Quando ele informa um usuário e senha válidos
E clica em "Entrar"
Então o sistema deve redirecionar para a tela inicial (dashboard)
```

**Passos executados:**
1.
2.
3.

**Resultado esperado:**

**Resultado obtido:**

**Status:** 🔲 Ainda não executado

**Evidência:** (print ou link do vídeo)

---

### Cenário 2: (variação negativa, ex. dado inválido)

```gherkin
Dado que o usuário está na tela de login do SIFIT
Quando ele informa uma senha incorreta
E clica em "Entrar"
Então o sistema deve exibir uma mensagem de erro
E não deve permitir o acesso
```

**Passos executados:**
1.
2.

**Resultado esperado:**

**Resultado obtido:**

**Status:** 🔲 Ainda não executado

**Evidência:**

---

### Checklist rápido

- [ ] Campos obrigatórios validados
- [ ] Mensagens de erro claras
- [ ] Dados refletidos corretamente no banco (validado via MySQL Workbench)
- [ ] Layout correto em diferentes tamanhos de tela (se aplicável)
