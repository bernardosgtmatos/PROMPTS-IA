## ESTRUTURA BASICA A SER SEGUIDA.

Todo prompt seguirá esta arquitetura testada e aprovada:

```markdown
1. **Papel da IA** (ex: "Atue como um Engenheiro Senior")
2. **Descrição em 1 frase do projeto**
3. **Escopo e Requisitos Detalhados** (em tópicos)
4. **Decisões Técnicas** (tecnologias sugeridas)
5. **Estratégia de Implementação** (passo a passo, pedindo validação a cada etapa)
6. **Mãos à obra!**
```

---

## 🎯 Exemplos Prontos para Você Usar

Abaixo estão **3 modelos de prompt** para diferentes tipos de projeto. Escolha o que mais se aproxima da ideia:

---

### 📌 Modelo 1: Aplicativo com Banco de Dados (ex: Sistema de Tarefas)

```markdown
Atue como um Desenvolvedor Full Stack. Vamos construir um aplicativo web de tarefas com banco de dados usando Vibe Coding.

**Descrição:**
"Um app de tarefas onde posso adicionar, editar, excluir tarefas e marcar como concluídas."

**Requisitos Detalhados:**
1.  Adicionar tarefa com título e descrição.
2.  Marcar tarefa como concluída/desconcluída.
3.  Editar título e descrição.
4.  Excluir tarefa.
5.  Filtrar: tarefas ativas, concluídas ou todas.
6.  Persistir dados no `localStorage`.

**Stack Técnica:**
- Frontend: HTML + TailwindCSS + Vanilla JS.
- Dados: `localStorage` (por simplicidade, depois podemos migrar para backend se precisar).

**Estratégia (confirme a cada passo):**
Passo 1: Estrutura HTML e CSS.
Passo 2: Função para salvar/carregar tarefas do localStorage.
Passo 3: Renderizar a lista de tarefas dinamicamente.
Passo 4: Implementar adicionar, editar, excluir.
Passo 5: Implementar filtros.
Passo 6: Adicionar animações/feedback visual para ações.

Vamos começar pelo Passo 1!
```

---

### 📌 Modelo 2: Dashboards e Relatórios (ex: Controle Financeiro)

```markdown
Atue como um Desenvolvedor Frontend com expertise em visualização de dados. Vamos construir um controle financeiro pessoal usando Vibe Coding.

**Descrição:**
"App para registrar despesas e receitas, com dashboard de gráficos e relatórios mensais."

**Requisitos:**
1.  Formulário para adicionar transações (valor, categoria, tipo: receita/despesa, data).
2.  Listar todas as transações com opção de editar/excluir.
3.  Dashboard com:
    - Saldo total.
    - Gráfico de pizza por categoria.
    - Gráfico de barras dos últimos 7 dias.
4.  Persistência: `localStorage` ou IndexedDB.

**Stack:**
- HTML + TailwindCSS
- Chart.js (para gráficos)
- Vanilla JS

**Estratégia:**
Passo 1: Estrutura base e formulário.
Passo 2: Funções de CRUD no localStorage.
Passo 3: Listar transações.
Passo 4: Calcular saldo e métricas.
Passo 5: Integrar Chart.js para gráficos.
Passo 6: Adicionar filtros por mês/ano.

Vamos nessa!
```

---

### 📌 Modelo 3: Automação e Scripts (ex: Organizador de Arquivos)

```markdown
Atue como um Especialista em Python e automação. Vamos criar um script de linha de comando para organizar arquivos usando Vibe Coding.

**Descrição:**
"Script que organiza arquivos de uma pasta em subpastas por extensão (ex: imagens, documentos, vídeos)."

**Requisitos:**
1.  Especificar a pasta alvo via argumento ou input.
2.  Mover arquivos para subpastas: `Imagens/`, `Documentos/`, `Videos/`, `Outros/`.
3.  Gerar um relatório do que foi movido.
4.  Opção de simulação (`--dry-run`) sem mover nada.
5.  Log de operações.

**Stack:**
- Python 3.8+
- Módulos padrão: `os`, `shutil`, `argparse`, `pathlib`

**Estratégia:**
Passo 1: Estrutura do script e parser de argumentos.
Passo 2: Mapear extensões para categorias.
Passo 3: Implementar função de mover com verificação.
Passo 4: Adicionar modo dry-run.
Passo 5: Gerar relatório em JSON e texto.
Passo 6: Criar arquivo de log.

Me mostre o código do Passo 1!
```

---

## 🔧 Como Adaptar Esses Modelos para Sua Ideia

Você pode modificar qualquer parte:

| Seção | O que você muda |
|-------|----------------|
| **Papel da IA** | "Atue como um Designer UI/UX", "Atue como um Cientista de Dados" |
| **Descrição** | Re-escreva sua ideia em 1 frase |
| **Requisitos** | Liste as funcionalidades do zero |
| **Stack** | Troque as tecnologias (React ao invés de Vanilla JS, Flask ao invés de HTML puro) |
| **Estratégia** | Ajuste os passos conforme sua lógica de construção |

---

## 💡 Dica de Ouro: O Prompt "Genérico Poderoso"

Se você não quiser usar um modelo específico, use este **super prompt genérico** que funciona para qualquer projeto:

```markdown
Vamos construir [NOME DO SEU PROJETO] usando Vibe Coding.

**Descrição:**
[Descreva sua ideia em 2-3 frases]

**Requisitos:**
[Liste cada funcionalidade como um item]

**Stack Preferida:**
[Mencione se tem preferência. Se não souber, peça: "Recomende a stack mais simples"]

**Decisões importantes:**
[Mencione algo crucial ex: "precisa funcionar offline", "precisa de login"]

**Estratégia:**
Divida em 6 passos lógicos e me peça validação antes de cada passo. O primeiro passo sempre será a estrutura base.

Pronto para começar?
```
