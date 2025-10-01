
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







































# Sistema de Cadastro de Empresas Parceiras – TechConnect Solutions

## 📌 Enunciado
A empresa **TechConnect Solutions** foi contratada para desenvolver um **Sistema de Cadastro de Empresas Parceiras** no prazo de **6 meses**.  
A equipe do projeto é composta por:  
- 1 Gerente de Projetos  
- 1 Analista de Sistemas  
- 2 Desenvolvedores  
- 1 Designer de Interface  
- 1 Tester (QA)  

O sistema deve contemplar:  
- Login com autenticação e recuperação de senha  
- Cadastro de empresas (CRUD)  
- Upload de logotipo  
- Relatórios em PDF/Excel  
- Painel administrativo com permissões  
- Interface responsiva  
- Banco de dados seguro e integrado  

O acompanhamento será feito por:  
- **Gráfico de Gantt**  
- **Metodologia Crystal Clear** com entregas incrementais  

---

## 📊 Gráfico de Gantt – Planejamento (6 meses)

```mermaid
gantt
    title Planejamento do Projeto - TechConnect Solutions
    dateFormat  YYYY-MM-DD
    section Levantamento e Planejamento
    Reunião inicial e requisitos     :a1, 2025-01-01, 7d
    Documentação funcional           :a2, after a1, 7d
    section Design
    Protótipos de telas              :b1, after a2, 7d
    Layout definitivo                :b2, after b1, 7d
    section Configuração inicial
    Ambiente + Git + BD              :c1, after b2, 7d
    section Desenvolvimento
    Módulo de Login                  :d1, after c1, 14d
    CRUD de empresas                 :d2, after d1, 14d
    Upload de logotipo               :d3, after d2, 14d
    Relatórios PDF/Excel             :d4, after d3, 14d
    Painel administrativo            :d5, after d4, 14d
    section Testes
    Testes unitários e integração    :e1, after d5, 28d
    Testes de usabilidade            :e2, after e1, 14d
    section Implantação
    Implantação final no servidor    :f1, after e2, 14d
    Validação e aceite do cliente    :f2, after f1, 7d






