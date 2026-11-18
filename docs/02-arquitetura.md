### Arquitetura

- 

---

### Fiação

#### Placa A 

| Função | GPIO | Observação |
|---|---|---|
| Botão de travessia | A16 | ... |
| LED vermelho externo | PTE30 | ... |
| LED verde externo | PTE29 | ... |
| Output PEDIDO | PTE23 | ... |
| Input CARROS_PARADO | PTE22 | ... |
| Input CARROS_PARADO | PTE21 | ... |

#### Placa B 

| Função | GPIO | Observação |
|---|---|---|
| Botão de modo | A16 | ... |
| LED vermelho externo| PTE30 | ... |
| LED verde externo | PTE29 | ... |
| Input PEDIDO | PTE23 | ... |
| Output CARROS_PARADO | PTE22 | ... |
| Output CARROS_PARADO | PTE21 | ... |

```mermaid
flowchart LR
    BTN_A(["🔘 Botão de travessia"])
    LR_A(["🔴 LED vermelho"])
    LG_A(["🟢 LED verde"])

    A["<b>Placa A</b>"]
    B["<b>Placa B</b>"]

    BTN_B(["🔘 Botão de modo"])
    LR_B(["🔴 LED vermelho"])
    LG_B(["🟢 LED verde"])

    BTN_A ---|PTA16| A
    LR_A ---|PTE30| A
    LG_A ---|PTE29| A

    A -->|"PEDIDO<br/>PTE23 → PTE23"| B
    B -->|"CARROS_PARADO<br/>PTE22 → PTE22"| A
    B -->|"CARROS_PARADO<br/>PTE21 → PTE21"| A
    A -.-|GND comum| B

    B ---|PTA16| BTN_B
    B ---|PTE30| LR_B
    B ---|PTE29| LG_B
```
