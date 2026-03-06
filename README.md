# 📒 Agenda de Contatos

## 📌 Descrição
Este projeto consiste no desenvolvimento de uma **agenda de contatos completa** como atividade final para o **Curso de Lógica de Programação**, com operações de **Adicionar**, **Editar**, **Pesquisar**, **Listar** e **Apagar** contatos.  

## Motivação e Incrementos Tecnológicos
A criação de uma agenda funcional serviu como ponto de partida. No entanto, a principal motivação e o esforço significativo foram direcionados para **superar um projeto base**, ainda que não seja um estudo avançado de programação, incorporando tecnologias e práticas mais avançadas que garantem uma experiência de melhor de uso, mecanismos de segurança de dados e manutenção facilitada. 
## As principais melhorias, que representam incrementos substanciais sobre uma solução básica, incluem:

## 🚀 Destaques Técnicos
- **Persistência de Dados (JSON)**: contatos salvos em `agenda_contatos.json`, garantindo integridade entre execuções.
- **Estrutura de Dados (Dicionários)**: armazenamento eficiente de Nome, Telefone e E-mail.
- **Validação Inteligente (`re`)**: telefones (11 dígitos) e e-mails verificados com expressões regulares.
- **Interface Amigável (ANSI)**: mensagens coloridas para títulos, erros, alertas e confirmações.
- **Exceção Personalizada**: `OperacaoCancelada` permite cancelar operações com segurança.
- **Limpeza de Tela Multiplataforma**: ajustada para funcionar em terminais locais e Colab.
- **Busca e Edição Flexíveis**: pesquisa insensível a maiúsculas/minúsculas e edição granular.
- **Confirmação de Ações Críticas**: exclusão e saída exigem confirmação explícita.

---

## 🖥️ Como Usar
1. **Execute o Notebook**: abra o arquivo `.ipynb` no Google Colab ou localmente com Python 3.x.  
2. **Interaja pelo Menu**: digite o número correspondente à ação desejada.  
3. **Cancelamento Seguro**: em qualquer entrada, digite `sair` para cancelar e retornar ao menu principal.  

---

## 🛠️ Tecnologias Utilizadas
- **Python 3.x**
- **Módulos Padrão**:
  - `re` (Expressões Regulares)  
  - `os` (Interação com o Sistema Operacional)  
  - `sys` (Interação com o Interpretador)  
  - `json` (Manipulação de Dados JSON)  

---

## 📂 Estrutura do Código
O projeto está organizado em funções independentes para cada operação:

- `carregar_agenda()` / `salvar_agenda()` → persistência de dados  
- `validar_formato()` / `validar_input()` → validação de entradas  
- `adicionar()` / `editar()` / `pesquisar()` / `apagar()` / `listar()` → operações principais  
- `limpar_tela()` → interface limpa e organizada  
- `executar_agenda()` → loop principal  

---

## ✅ Exemplo de Uso
```bash
===== AGENDA DE CONTATOS =====
1 - Adicionar novo contato
2 - Editar contato
3 - Pesquisar contato
4 - Listar contatos
5 - Apagar um contato
6 - Sair
