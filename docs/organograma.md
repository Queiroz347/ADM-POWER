# Organograma (versão ajustável)

Você tinha razão: agora também deixei **a imagem do organograma** no repositório.

![Organograma ajustado](./organograma.svg)

Arquivo da imagem: `docs/organograma.svg`.

## Visão geral editável (Mermaid)

```mermaid
flowchart LR
    CHMDT["CHMDT\nGerente"]
    GESTAO["Gestão Operacional"]
    PLANEJAMENTO["Planejamento"]
    PM["PM / Portfólio"]
    DE["Diretoria Executiva"]

    CHMDT --> GESTAO
    CHMDT --> PLANEJAMENTO
    CHMDT --> PM
    CHMDT --> DE

    subgraph EQUIPE_CAMPO["Fiscalização de Campo"]
      SUP1["Supervisor 1"] --> TEC11["Técnico 1"]
      SUP1 --> TEC12["Técnico 2"]
      SUP2["Supervisor 2"] --> TEC21["Técnico 3"]
      SUP2 --> TEC22["Técnico 4"]
      SUP3["Supervisor 3"] --> TEC31["Técnico 5"]
      SUP3 --> TEC32["Técnico 6"]
    end

    GESTAO --> EQUIPE_CAMPO
```

## Como ajustar rapidamente

1. Para editar visualmente, abra `docs/organograma.svg` em qualquer editor SVG (Figma, Inkscape, Illustrator, etc.).
2. Para editar em texto, ajuste o bloco Mermaid acima.
3. Para exportar PNG/PDF, use o próprio editor SVG.
