# Cenário de Teste — Login

> 🔲 **Status: ainda não iniciado.** Cenários redigidos, mas nenhum foi executado ainda no sistema.

**Funcionalidade:** Autenticação (Login)

**Tipo de teste:** Funcional / Positivo / Negativo

**Requisito relacionado:** RF-01 (ver `1-Analise de requisitos.md`)

---

### Cenário 1: Login com credenciais válidas (positivo)

```gherkin
Dado que o usuário está na tela de login (sifit.centrion.com.br/login)
Quando ele informa um usuário e senha válidos
E clica em "Entrar"
Então o sistema deve autenticar o usuário
E redirecionar para a tela inicial do sistema
```

**Passos executados:**
1. Acessar `sifit.centrion.com.br/login`
2. Preencher usuário e senha válidos
3. Clicar em "Entrar"

**Resultado esperado:** Acesso liberado, usuário direcionado à tela inicial.

**Resultado obtido:** (preencher após execução)

**Status:** 🔲 Ainda não executado

**Evidência:** (print com a senha oculta, ou link do vídeo gravado com a extensão Jam)

---

### Cenário 2: Login com senha incorreta (negativo)

```gherkin
Dado que o usuário está na tela de login
Quando ele informa um usuário válido e uma senha incorreta
E clica em "Entrar"
Então o sistema deve exibir uma mensagem de erro
E não deve conceder acesso
```

**Passos executados:**
1. Acessar a tela de login
2. Preencher usuário válido e senha incorreta
3. Clicar em "Entrar"

**Resultado esperado:** Mensagem de erro exibida, acesso negado.

**Resultado obtido:** (preencher após execução)

**Status:** 🔲 Ainda não executado

**Evidência:**

---

### Cenário 3: Campos obrigatórios vazios (negativo)

```gherkin
Dado que o usuário está na tela de login
Quando ele clica em "Entrar" sem preencher usuário e senha
Então o sistema deve impedir o envio
E indicar quais campos são obrigatórios
```

**Passos executados:**
1. Acessar a tela de login
2. Clicar em "Entrar" sem preencher nada

**Resultado esperado:** Sistema não envia o formulário e sinaliza os campos obrigatórios.

**Resultado obtido:**

**Status:** 🔲 Ainda não executado

**Evidência:**

---

### Cenário 4: "Esqueci minha senha" (exploratório)

```gherkin
Dado que o usuário está na tela de login
Quando ele clica em "Esqueci minha senha"
Então o sistema deve apresentar um fluxo de recuperação de senha
```

**Resultado esperado:**

**Resultado obtido:**

**Status:** 🔲 Ainda não executado

**Evidência:**

---

### Checklist rápido

- [ ] Login válido funciona
- [ ] Login inválido é bloqueado com mensagem clara
- [ ] Campos obrigatórios validados
- [ ] Opção "Manter conectado" funciona como esperado
- [ ] Fluxo "Esqueci minha senha" funciona
