# DAS (v0.1)

Drone Automation System

### Introdução

Sistema para automação e inteligencia artificial de drones. O sistema funciona em cima de outros sistemas de voo e piloto automatico captando dados com sensores e tomando decisões mais complexas como desviar de objetos e recalcular trajetorias, alem de auxiliar na captura de imagens e de dados com sensores. 

### Features

* Sensores que capturam uma nuvem de pontos do ambiente
* Proteção contra colisões (modo piloto automatico e voo assistido)
* Controle do Payload via tracking
* Caixa preta
* Telemetria encriptada via multiplos protocolos


### Funcionamento

O sistema de automação de drones funciona como um processo separado que controla o sistema de voo. O DAS fica captando e processando dados com seus sensores e faz previsões de colisão. Ao indentificar uma possivel colisão o DAS desliga o piloto automatico do sistema de voo e controla a aeronave manualmente até ela passar pelo obstaculo. Em seguida o piloto automatico é ligado novamente e aeronave volta para sua rota inicial.

Alem disso o DAS funciona como um sistema de auxilio a missão. Ele controla o payload para captura de imagens ou dados e se sertifica que os dados são validos. Se necesseario, o DAS toma controle do voo da nave e a reposiciona para recapturar os dados até que eles sejam validos.

O DAS também funciona como um sistema de proteção contra colisões no caso de voo manual com um operador. Necesse caso ele funciona como um assistente de voo e no caso de colisão eminente o sistema toma total controle da aeronave.

### Hardware

- 3DR Pixhawk ou PX4FMU+I/O
- RaspberryPi
- GPS
- PX4-Flow (camera + sensor ultrasonico)
- Magnetometro
- WindSpeed Sensor
- Hokuyo URG-04LX-UG01 Scanning Laser Rangefinder
- MESA Imaging 3D ToF Camera SR4000

### Equipe

- James Peret
- Estevão Trabbold

