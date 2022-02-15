# Mermaid Markdown Samples

Samples from https://mermaid-js.github.io/mermaid

- [Flowchart](https://github.com/junkofujiwara/mermaid-md-samples/blob/main/flowchart.md)
```mermaid
flowchart LR;
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
```
- [Sequence Diagram](https://github.com/junkofujiwara/mermaid-md-samples/blob/main/sequence-diagram.md)
```mermaid
sequenceDiagram
    autonumber
    Alice->>John: Hello John, how are you?
    loop Healthcheck
        John->>John: Fight against hypochondria
    end
    Note right of John: Rational thoughts!
    John-->>Alice: Great!
    John->>Bob: How about you?
    Bob-->>John: Jolly good!
```
- [Class Diagram](https://github.com/junkofujiwara/mermaid-md-samples/blob/main/class-diagram.md)
```mermaid
classDiagram
    direction RL
  class Student {
    -idCard : IdCard
  }
  class IdCard{
    -id : int
    -name : string
  }
  class Bike{
    -id : int
    -name : string
  }
  Student "1" --o "1" IdCard : carries
  Student "1" --o "1" Bike : rides
```
- [State Diagram](https://github.com/junkofujiwara/mermaid-md-samples/blob/main/state-diagram.md)
```mermaid
stateDiagram
    direction LR
    [*] --> A
    A --> B
    B --> C
    state B {
      direction LR
      a --> b
    }
    B --> D
```

References
- [About Mermaid](https://mermaid-js.github.io/mermaid)
- [About writing and formatting on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github)
- [Include diagrams in your Markdown files with Mermaid](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)
