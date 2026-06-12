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
distribuição por estado/tribunal/ano, status, fase, aging, mapa de êxito produto × UF,
desempenho por produto/UF/litigante e drill-down de todos os processos.

> Documento interno de gestão.
