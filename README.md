# Sistema Inteligente de Monitoramento da Qualidade da Água – IoT (ODS 6)

Este projeto consiste em um protótipo funcional de um sistema inteligente para monitoramento da qualidade da água, utilizando sensores físicos, microcontrolador e comunicação via protocolo MQTT.

## 🌐 Objetivo

Apoiar o cumprimento do ODS 6 da ONU, promovendo o uso sustentável da água com tecnologia de IoT.

## 🛠 Componentes Utilizados

- NodeMCU ESP8266 (ou Arduino Uno + comunicação serial)
- Sensor de Temperatura (NTC)
- Sensor de Turbidez
- Sensor de TDS
- Sensor de pH (substituído por potenciômetro para simulação)
- Display LCD 16x2
- Válvula solenoide (simulada)
- Bomba d’água (simulada)
- Jumpers, protoboard, fonte de alimentação

## 🔗 Comunicação via MQTT

A comunicação entre o dispositivo e a nuvem é realizada via protocolo **MQTT**, utilizando o **Mosquitto Broker**. Os dados são publicados nos seguintes tópicos:

- `agua/temperatura`
- `agua/turbidez`
- `agua/tds`
- `agua/ph`
- `agua/status`

## 💻 Como rodar

1. Instale a IDE do Arduino e as bibliotecas necessárias (`LiquidCrystal`, `PubSubClient`, `ESP8266WiFi`, se NodeMCU).
2. Configure o Wi-Fi e o endereço do broker no código.
3. Faça upload para a placa.
4. Abra o monitor serial para visualizar os dados.
5. Acompanhe a comunicação em tempo real com um cliente MQTT (ex: MQTT Explorer, Node-RED, etc).

## Resultados

- Tempo médio de resposta dos sensores e atuadores: veja em [docs/relatorio_medições.xlsx](docs/relatorio_medições.xlsx)
- Dados visuais da montagem estão disponíveis em [imagens/](imagens)
- Fluxograma de funcionamento: [imagens/fluxograma.png](imagens/fluxograma.png)

## Vídeo Demonstração

Assista ao vídeo completo da demonstração do projeto no YouTube (modo não listado):
🔗 [Clique aqui para assistir](https://youtube.com/SEU-LINK-AQUI)

## Artigo

Disponível em [docs/artigo_final.pdf](docs/artigo_final.pdf)

## Esquemas

O esquema eletrônico pode ser encontrado em [esquemas/fritzing_esquema.fzz](esquemas/fritzing_esquema.fzz)

## Licença

Este projeto é livre para fins educacionais.
