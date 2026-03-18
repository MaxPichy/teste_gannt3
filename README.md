```mermaid
  gantt
  %%%Definir título principal
  title Desenvolvimento de Software

  %%%Definir o formato data (Ano-Mês-Dia)
  dateFormat YYYY-MM-DD

  %%%Criação do agrupamento visual para as tarefas iniciais
  section Planejamento

  %%%'done': 'tarefa concluída(fica cinza)', 'req': 'id da tarefa', '2026-03-11': 'data de início', '10d': 'duração'
  Requisitos :done, req, 2026-03-11, 10d

  %%%'active': 'tarefa em andamento'
  Design :active, des, 2026-03-20, 15d

  %%%Criação do segundo bloco
  section Desenvolvimento

  %%%'crit': 'define como tarefa crítica (cor vermelha ou destaque)'
  Codificação :crit, dev, 2026-03-25, 30d

  %%%'after dev': 'realiza a tarefa quando a tarefa dev terminar'
  Teste :test, after dev, 15d

  section Lançamento
  Implantação :dep, after test, 5d
  Treinamento : tra, after dep, 10d
```


```mermaid
  graph TD
  subgraph Matriz

  A1["Refatorar 2"]:::branco-->
  A2["Comunicação Banco 5"]:::laranja-->
  A3["Conexão Internet 2"]:::vermelho

  B1["M Design 1"]:::branco-->
  B2["N Backup"]:::laranja-->
  B3["N Servidor"]:::vermelho
  end
  
  classDef branco color:#000, fill:#FFF, stroke:#000, stroke-width:1px;
  classDef laranja color:#000, fill:#FFA233, stroke:#000, stroke-width:1px;
  classDef vermelho color:#000, fill:#FF0000, stroke:#000, stroke-width:1px;
  

```


