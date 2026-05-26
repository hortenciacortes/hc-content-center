# .github/rules/frontend-rules.md

## Diretrizes Técnicas (aplicar sempre)

- Componentes Angular devem ser `standalone: true`.
- Componentes devem usar `ChangeDetectionStrategy.OnPush`.
- Preferir injeção por propriedade com `inject()` e modificadores explícitos (`public/private readonly`) quando aplicável.
- Templates devem priorizar control flow novo do Angular (`@if`, `@for`, `@switch`).
- Seguir convenções de quebra de linha/ordenação definidas no `CODERULES.md` (incluindo arrays de `imports`).
- Você utiliza o ESLint para garantir qualidade e consistência do código. Sempre corrija os erros de lint antes de finalizar a tarefa.
- Você segue os padrões es6+ para escrita de código, incluindo uso de `const`/`let`, arrow functions, template literals, destructuring, etc.
- Você tem conhecimento avançado de TypeScript e Angular, incluindo conceitos como RxJS, Observables, Dependency Injection, Change Detection, etc.
- Você é capaz de ler e entender código Angular complexo, identificar padrões e aplicar boas práticas de desenvolvimento frontend.
- Você é capaz de escrever código Angular limpo, eficiente e de fácil manutenção, seguindo as convenções do projeto e as melhores práticas do setor.
- Evitar criar variáveis e funções novas que venham a aumentar a complexidade do código, a menos que sejam realmente necessárias para resolver o problema em questão. Priorizar soluções simples e diretas.
- Escrever testes unitários para as mudanças implementadas, garantindo que o código esteja coberto e que as funcionalidades estejam funcionando como esperado. Seguir os padrões de teste já existentes no projeto para manter consistência.

## Componentes

* Componentes devem possuir responsabilidade única.
* Evitar componentes excessivamente grandes.
* Extrair componentes reutilizáveis apenas quando houver reutilização real.
* Evitar lógica complexa diretamente no template.

---

# Formulários

* Utilizar Reactive Forms.
* Toda validação deve possuir feedback visual.
* Inputs devem ser tipados.
* Evitar uso de any.

---

# Estado

* Priorizar soluções simples.
* Utilizar Signals quando fizer sentido.
* Utilizar RxJS sem complexidade desnecessária.
* Evitar gerenciamento global de estado para o MVP.

---

# HTTP e Serviços

* Separar chamadas HTTP em services.
* Tratar loading, erro e estado vazio.
* Centralizar tratamento de erros quando possível.

---

# Organização

* Utilizar arquitetura baseada em features.
* Shared deve conter apenas itens realmente compartilhados.
* Core deve conter serviços globais e infraestrutura.

---

# UI/UX

* Priorizar clareza visual.
* Sempre tratar:
  * loading
  * erro
  * empty state
* Manter consistência visual.

---

# Código

* Priorizar legibilidade.
* Comentários apenas quando realmente necessários.
* Evitar abstrações prematuras.
* Preferir código simples e explícito.


# Commit Message Convention

Todas as mensagens de commit devem iniciar obrigatoriamente com um dos seguintes prefixos:

**ADD**
**UPDATE**
**REMOVE**
**FIX**

**Formato:**
TYPE: descrição curta e objetiva

**Exemplos:**

ADD: create posts dashboard
ADD: implement markdown preview
UPDATE: improve loading state handling
UPDATE: refactor post form structure
FIX: correct slug generation bug
FIX: resolve empty state rendering
REMOVE: delete unused shared component

**Regras**
- Mensagens devem ser escritas em inglês.
- Utilizar verbos objetivos.
- Evitar commits genéricos.
- Descrição deve ser curta e clara.
- Um commit deve representar uma mudança coesa.

**Significado dos Prefixos**

**ADD**

Nova funcionalidade, componente, página ou feature.

**UPDATE**

Melhoria, refatoração ou alteração em funcionalidade existente.

**FIX**

Correção de bug ou comportamento incorreto.

**REMOVE**

Remoção de código, componente, arquivo ou funcionalidade.

## Formato de resposta esperado

- Respostas curtas, diretas e acionáveis.
- Sempre informar:
	- o que foi alterado,
	- onde foi alterado,
	- como validar,
	- e eventuais riscos/pendências.

