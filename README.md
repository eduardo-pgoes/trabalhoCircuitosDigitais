# Panda - SmartSprinkle
Esse é o repositório Git que armazena os arquivos do projeto SmartSprinkle, feito por Victor Yo Yin (RA 164003) e Eduardo Goes (RA 156465) para a disciplina de Circuitos Digitais.

# Instruções para execução
## Pré-Requisitos
- Instalação do [WiredPanda](https://gibis-unifesp.github.io/wiRedPanda/)

## Estrutura do Projeto
O arquivo principal do projeto se chama `ProjetoPrincipal.panda`. Todos os outros arquivos são CIs para subcircuitos.

Segue uma relação dos inputs:

| Nome do Input | Descrição                                                      |
|---------------|----------------------------------------------------------------|
| UmidadeA0     | Bit menos significativo do sensor de umidade da zona A         |
| UmidadeB0     | Ver acima - para a zona B                                      |
| UmidadeA1     | Segundo bit menos significativo do sensor de umidade da zona A |
| UmidadeB1     | Ver acima - para a zona B                                      |
| UmidadeA2     | 3o bit do sensor de umidade da zona A |
| UmidadeB2     | Ver acima - para a zona B                                      |
| UmidadeA3     | 4o bit do sensor de umidade da zona A |
| UmidadeB3     | Ver acima - para a zona B                                      |
| UmidadeA4     | Bit mais significativo do sensor de umidade da zona A |
| UmidadeB4     | Ver acima - para a zona B                                      |
| Chuva         | Sensor de presença de chuva - 1 significa que está chovendo, 0 significa que não                                      |
| PulsoResetDiario         | Deve ser setado para 0 (e retornado para 1) uma vez ao dia - simula um pulso RTC |
| Temperatura0     | Bit menos significativo do sensor de temperatura         |
| Temperatura1     | Segundo bit menos significativo do sensor de temperatura         |
| Temperatura2     | 3o bit do sensor de temperatura         |
| Temperatura3     | 4o bit do sensor de temperatura         |
| Temperatura4     | Bit mais significativo do sensor de temperatura         |

Por fim, dos outputs:

| Nome do Output | Descrição                                                      |
|---------------|----------------------------------------------------------------|
| ZonaSelecionada     | 1 = zona A, 0 = zona B         |
| AcionarAlarme     | Descreve o estado do alarme de condições para irrigação duplicadas |
| AcionarBomba     | Descreve o estado da bomba - se deve ou não ser ativada |
| Intensidade0     | Bit menos significativo da intensidade do motor da bomba |
| Intensidade1     | Segundo bit menos significativo da intensidade do motor da bomba |
| Intensidade2     | 3o bit da intensidade do motor da bomba                 |
| Intensidade3     | Bit mais significativo da intensidade do motor da bomba |