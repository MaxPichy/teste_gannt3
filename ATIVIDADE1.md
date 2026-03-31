```mermaid
  gantt
  title TechConnect Solutions
  subtitle Sistema de Cadastro de Empresas Parceiras
  dateFormat YYYY-MM-DD

  section Requisitos
  Levantamento: active, req, 2026-04-01, 7d
  Documentação: after req, doc, 7d

  section Design
  Modelos: after doc, mod, 7d
  Layout Final: after mod, lay, 14d  

  section Desenvolvimento
  Configuração: after doc, cfg, 4d
  Banco de Dados: after cfg, bd, 14d
  Login: after bd, lgn, 7d
  CRUD: after bd, crd, 7d
  Logotipo: after crd, lgt, 7d
  Exportações: after lgt, exp, 7d
  Administração: after exp, adm, 7d
  Correções: after re1, cor, 21d
  Implementação: deploy, after vsb, 7d

  section Testes
  Testes: after adm, tst, 14d
  Relatório: after tst, re1, 3d
  Versão Beta: after cor, vsb, 7d

``
