# Plano de Testes — Cruzamento com Semáforos de Veículos e Pedestres

Abreviações: TU - testes de unidade; TIS - testes de integração / sistema; TV - teste de validação

Plano de verificação seguindo o **modelo V**:

### Testes de unidade

- [ ] TU01: validar o semáforo de pedestres normal (verde acende por 4 segundos, vermelho acende por 4 segundos)
- [ ] TU02: validar o semáforo de veículos normal (verde acende por 3 segundos, amarelo acende por 1 segundo, vermelho acende por 4 segundos)
- [ ] TU03: validar o semáforo de pedestres noturno (vermelho piscando a cada 2 segundos)
- [ ] TU04: validar o semáforo de veículos noturno (amarelo piscando a cada 2 segundos)
- [ ] TU05: validar o botão 
- [ ] TU06: validar a comunicação entre as placas

### Testes de integração / sistema

- [ ] TIS01: validar o modo normal 
- [ ] TIS02: validar modo noturno
- [ ] TIS03: validar o modo normal com botão de travessia
- [ ] TIS04: validar integração entre modo normal e noturno
- [ ] TIS05: validar integração entre modo normal e noturno com 1 botão de travessia
- [ ] TIS06: validar modo normal com duas placas
- [ ] TIS07: validar modo normal com duas placas e 2 botões de travessia
- [ ] TIS08: validar modo noturno com duas placas
- [ ] TIS09: validar modo normal e noturno com duas placas

### Testes de validação

- [ ] TV01: validar modo normal e noturno com duas placas e 2 botões de travessia
