# micro-frontend

```mermaid
graph TD;
    subgraph Shell Application
        A[Shell (Container App)]
    end

    subgraph Application1
        B1[Application1]
        C1[Micro Frontend Component 1]
        C2[Micro Frontend Component 2]
    end

    subgraph Application2
        B2[Application2]
        C3[Micro Frontend Component 3]
        C4[Micro Frontend Component 4]
    end

    subgraph Remote Components
        R1[Remote Component 1]
        R2[Remote Component 2]
        R3[Remote Component 3]
        R4[Remote Component 4]
    end

    A -->|Loads| B1
    A -->|Loads| B2
    B1 -->|Uses| C1
    B1 -->|Uses| C2
    B2 -->|Uses| C3
    B2 -->|Uses| C4

    C1 -->|Fetches| R1
    C2 -->|Fetches| R2
    C3 -->|Fetches| R3
    C4 -->|Fetches| R4

```
