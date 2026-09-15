# Rastreabilidade de IA

| Pedido ao agente | Aceito/rejeitado | Justificativa técnica e verificação |
|---|---|---|
| Implementar as regras de alerta dos sensores de nível e temperatura | Aceito | Nível entra em alerta abaixo de 20% e temperatura acima de 45°C, conforme o contrato da atividade. |
| Implementar a formatação do painel em C++ e Python | Aceito | O painel consulta o contrato do sensor e mostra valor, unidade e estado com uma casa decimal. |
| Manter a pressão reservada para a Etapa 02 | Aceito | A implementação da pressão não foi alterada, pois sua validação está prevista para a próxima etapa. |
| Verificar a implementação da Etapa 01 | Aceito | `make run` funcionou em C++ e Python e `make test ETAPA=01` terminou com `OK (skipped=1)`, sendo o teste da pressão reservado para a Etapa 02. |
