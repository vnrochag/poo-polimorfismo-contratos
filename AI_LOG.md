# Rastreabilidade de IA

| Pedido ao agente | Aceito/rejeitado | Justificativa técnica e verificação |
|---|---|---|
| Implementar as regras de alerta dos sensores de nível e temperatura | Aceito | Nível entra em alerta abaixo de 20% e temperatura acima de 45°C, conforme o contrato da atividade. |
| Implementar a formatação do painel em C++ e Python | Aceito | O painel consulta o contrato do sensor e mostra valor, unidade e estado com uma casa decimal. |
| Manter a pressão reservada para a Etapa 02 | Aceito | A implementação da pressão não foi alterada na Etapa 01, pois sua validação estava prevista para a próxima etapa. |
| Verificar a implementação da Etapa 01 | Aceito | `make run` funcionou em C++ e Python e `make test ETAPA=01` terminou com `OK (skipped=1)`, sendo o teste da pressão reservado para a Etapa 02. |
| Implementar o sensor de pressão em C++ e Python | Aceito | A pressão aceita valores finitos de 0 a 10 bar e rejeita valores fora desse intervalo, preservando o estado anterior. |
| Implementar o alerta do sensor de pressão | Aceito | A pressão entra em alerta somente quando o valor é maior que 8 bar. |
| Verificar a Etapa 02 | Aceito | `make test ETAPA=02` passou em C++ e Python, e `make run` mostrou a pressão em 8.5 bar com estado ALERTA nos dois casos. |
| Atualizar o diagrama de classes | Aceito | O diagrama representa Sensor como classe abstrata, as três especializações e a dependência do Painel pelo contrato de Sensor. |
