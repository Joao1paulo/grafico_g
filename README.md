
```mermaid
flowchart TD

  A(["Início"])
  A --> B{"Faça uma escolha"}
  B --> C["OP1"]
  B --> D["OP2"]
  B --> E["OP3"]
```

```mermaid
graph TD;
A[Inicio] --> B{Nota >6};
B --> |SIM| C[Aprovado];
B --> |NÃO| D[Reprovado];
```

```mermaid
gantt
title Exemplo de Gráfico de Gantt
dateFormat YYYY-MM-DD
section 1°Semestre
1°Bimestre ✅Concluido: done, a1, 2025-02-02, 60d
2°Bimestre ✅Concluido: done, a2, after a1, 60d

section 2° Bimestre
3° Bimestre ⌛Em Andamento: active, a3, 2025-08-01, 60d
4° Bimestre ➡️Em Andamento: crit, a4, after a3, 60d
```



```mermaid
graph TD
  subgraph Matriz
A1["UX C3"]:::branco --> A2["C20"]:::amarelo --> A3["V5O"]:::laranja --> A4["V100"]:::vermelho
B1["UX C9"]:::branco --> B2["E20"]:::amarelo --> B3["E50"]:::laranja --> B4["E100"]:::vermelho
C1["D8"]:::branco --> C2["D20"]:::amarelo --> C3["D50"]:::laranja --> C4["BD V 89"]:::vermelho
D1["C8"]:::branco --> D2["C20"]:::amarelo --> D3["C50"]:::laranja --> D4["BD V 100"]:::vermelho
end
classDef branco fill:#fff, stroke:#o00, stroke-width:1px;
classDef amarelo fill:#FFD8D, stroke:#oeo, stroke-width:1px;
classDef laranja fill:#FFA233, stroke:#000, stroke-width:1px;
classDef vermlho fill:#E64C3C, stroke:#000, stroke-width:1px;
```

---


```mermaid
gantt
title Estudo de Caso - Construção de uma Casa
dateFormat YYYY-MM-DD

section Planejamento
Preparação de Desenhos Arquitetônicos, Aprovações e Plano de Construção ✅Concluído :done, a1, 2025-01-01, 20d

section Terreno
Preparação do Terreno ⌛Em Andamento :active, a2, after a1, 10d

section Estrutura
Fundação ➡️Pendente :crit, a3, after a2, 15d
Estrutura da Casa :a4, after a3, 30d

section Instalações
Instalações Elétricas e Hidráulicas :a5, after a4, 20d

section Acabamentos
Acabamento Interno :a6, after a5, 25d
Acabamento Externo :a7, after a6, 15d

section Entrega
Inspeção Final e Entrega :a8, after a7, 5d

```



<!-- ```mermaid
gantt
title Construção de uma Casa
dateFormat YYYY-MM-DD
section Planejamento
Planejamento e Aprovações ✅:done, a1, 2025-01-01, 20d

section Terreno
Preparação do Terreno ⌛:active, a2, after a1, 10d

section Estrutura
Fundação ➡️:crit, a3, after a2, 15d
Estrutura da Casa :a4, after a3, 30d

section Instalações
Instalações Elétricas e Hidráulicas :a5, after a4, 20d

section Acabamentos
Acabamento Interno :a6, after a5, 25d
Acabamento Externo :a7, after a6, 15d

section Entrega
Inspeção Final e Entrega :a8, after a7, 5d
``` -->

<!-- ```mermaid
gantt
    title Gráfico de Gantt - Sistema de Cadastro de Empresas Parceiras
    dateFormat  YYYY-MM-DD
    axisFormat  %Y-%m-%d
    
    section Pré-Desenvolvimento (Planejamento)
    Levantamento de Requisitos e Documentação :a1, 2025-10-01, 10d
    Elaboração de Rascunhos e Layout UI/UX :a2, after a1, 8d
    
    section Fase de Desenvolvimento I (Entregas 1, 2 e 3)
    Configuração do Ambiente e DB (Setup) :d1, after a2, 5d
    Programação Módulo Login (Entrega 1 - Semana 3) :d2, after d1, 10d
    Programação CRUD de Empresas (Entrega 2 - Semana 6) :d3, after d2, 15d
    Implementação do Upload de Logotipo (Entrega 3 - Semana 8) :d4, after d3, 10d
    
    section Fase de Desenvolvimento II (Entregas 4 e 5)
    Desenvolvimento dos Relatórios (Entrega 4 - Semana 10) :d5, after d4, 10d
    Configuração Painel Admin e Permissões (Entrega 5 - Semana 12) :d6, after d5, 10d

    section Testes e Implantação (Entrega Final - Mês 6)
    Testes Unitários e de Integração (QA) :t1, after d6, 15d
    Testes de Usabilidade com Usuários Convidados :t2, after t1, 10d
    Correções e Ajustes Finais :i1, after t2, 10d
    Implantação Final no Servidor e Entrega ao Cliente (Mês 6) :i2, after i1, 5d
``` -->



