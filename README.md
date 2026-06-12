# Processos Judiciais — BM Advocacia & Consultoria

Painel de controladoria processual da Borges Macedo Advocacia e Consultoria.

**Acesso:** https://borgesmacedoadvocacia.github.io/processosjudiciais

## Como funciona
Dashboard estático (HTML único) hospedado no GitHub Pages. Os dados são lidos **ao vivo**
da planilha Google Sheets «Clientes e Processos – BM Advocacia», aba *Todos os Processos*,
via endpoint público `gviz/tq` — a cada carregamento e ao clicar em **Atualizar**.
Não há dados congelados no repositório.

### Sincronização
- A planilha precisa estar compartilhada como **«qualquer pessoa com o link pode ver»**.
- Qualquer alteração na planilha aparece no painel ao recarregar a página.

### Métricas
Êxito sob a ótica do cliente, deferimento de liminar, reforma em 2º grau, taxa de acordo,
pendências (de julgamento, de recurso, de liminar), distribuição por estado/tribunal/ano,
status, fase, aging, cascata processual, mapa de êxito produto × UF, desempenho por
produto/UF/litigante, intervalos de confiança de Wilson e drill-down de todos os processos.

### Consultor IA
A aba **Consultor IA** responde perguntas objetivas sobre os dados (ex.: "quantas ações de
revisional de plano de saúde estão ativas e ainda sem alvará creditado?"). O Claude interpreta
a pergunta e o navegador calcula a contagem exata na base — números nunca são estimados.

- Requer uma **chave da API do Claude** (console.anthropic.com), inserida pelo próprio usuário
  e guardada **apenas no navegador** (localStorage). A chave **nunca** é versionada no repositório.
- A conexão usa o endpoint `/v1/messages` com tool use, direto do navegador.

> Documento interno de gestão.
