### Graph [Reference](https://mermaid-js.github.io/mermaid/#/flowchart?id=graph)

```mermaid
flowchart TD;
    Start --> Stop;
```

```mermaid
flowchart LR;
    Start --> Stop;
```


```mermaid
flowchart BT;
    Start --> Stop;
```

```mermaid
flowchart RL;
    Start --> Stop;
```

### Node shapes [Reference](https://mermaid-js.github.io/mermaid/#/flowchart?id=node-shapes)

```mermaid
flowchart LR;
    id1(This is the text in the box)
```

```mermaid
flowchart LR;
    id1([This is the text in the box])
```

```mermaid
flowchart LR;
    id1[[This is the text in the box]]
```

```mermaid
flowchart LR;
    id1[(Database)]
```

```mermaid
flowchart LR;
    id1((This is the text in the circle))
```

```mermaid
flowchart LR;
    id1>This is the text in the box]
```

```mermaid
flowchart LR;
    id1{This is the text in the box}
```

```mermaid
flowchart LR;
    id1{{This is the text in the box}}
```

```mermaid
flowchart LR;
    id1[/This is the text in the box/]
```

```mermaid
flowchart LR;
    id1[\This is the text in the box\]
```

```mermaid
flowchart LR;
    A[/Trapezoid\]
```
```mermaid
flowchart LR;
    B[\Go shopping/]
```


### Links [Reference](https://mermaid-js.github.io/mermaid/#/flowchart?id=links-between-nodes)

```mermaid
flowchart LR;
    A-->B
```

```mermaid
flowchart LR;
    A --- B
```

```mermaid
flowchart LR;
     A-- This is the text! ---B
```

```mermaid
flowchart LR;
    A-->|text|B
```

```mermaid
flowchart LR;
    A-- text -->B
```

```mermaid
flowchart LR;
    A-.->B;
```

```mermaid
flowchart LR;
    A-. text .-> B
```

```mermaid
flowchart LR;
    A ==> B
```

```mermaid
flowchart LR;
    A == text ==> B
```

```mermaid
flowchart LR;
    A -- text --> B -- text2 --> C
```

```mermaid
flowchart LR;
    a --> b & c--> d
```

```mermaid
flowchart LR;
    A & B--> C & D
```

```mermaid
flowchart LR;
    A --o B
    B --x C
```

```mermaid
flowchart LR;
    A o--o B
    B <--> C
    C x--x D
```

```mermaid
flowchart LR;
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
```

### Subgraphs [Reference](https://mermaid-js.github.io/mermaid/#/flowchart?id=subgraphs)

```mermaid
flowchart TB;
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

```mermaid
flowchart TB;
    c1-->a2
    subgraph ide1 [one]
    a1-->a2
    end
```

```mermaid
flowchart TB;
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
    one --> two
    three --> two
    two --> c2
```

```mermaid
flowchart LR
  subgraph TOP
    direction TB
    subgraph B1
        direction RL
        i1 -->f1
    end
    subgraph B2
        direction BT
        i2 -->f2
    end
  end
  A --> TOP --> B
  B1 --> B2
```

### Styling [Reference](https://mermaid-js.github.io/mermaid/#/flowchart?id=styling-and-classes)

```mermaid
flowchart LR
    id1(Start)-->id2(Stop)
    style id1 fill:#f9f,stroke:#333,stroke-width:4px
    style id2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```
