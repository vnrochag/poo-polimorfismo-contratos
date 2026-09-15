# Diagrama de classes

Sensor (abstrata)
- tag()
- valor() [abstrata]
- unidade() [abstrata]
- atualizar(leitura) [abstrata]
- emAlerta() [abstrata]

SensorNivel
- valor()
- unidade()
- atualizar(leitura)
- emAlerta()

SensorTemperatura
- valor()
- unidade()
- atualizar(leitura)
- emAlerta()

SensorPressao
- valor()
- unidade()
- atualizar(leitura)
- emAlerta()

Painel
- linhaPainel(Sensor)

Relações:
- SensorNivel herda de Sensor
- SensorTemperatura herda de Sensor
- SensorPressao herda de Sensor
- Painel depende de Sensor
- O Painel recebe uma referência para Sensor e não possui os sensores