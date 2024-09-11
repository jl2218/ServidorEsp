# Projeto de Controle de Lâmpada com ESP32

Este projeto demonstra como controlar uma lâmpada (ou LED embutido) usando um ESP32 como servidor local. A interface para o controle é baseada em HTML, permitindo que você acenda e apague a lâmpada através de um navegador web.

## Visão Geral

O ESP32 é programado para conectar-se a uma rede Wi-Fi existente e servir uma página HTML que permite ao usuário controlar um LED conectado ao dispositivo. O código em C++ (Arduino) configura o ESP32 para hospedar um servidor web com endpoints para acender e apagar o LED.

## Requisitos

- **ESP32**: Placa de desenvolvimento.
- **LED**: LED ou lâmpada conectada ao pino configurado no ESP32.
- **Cabo USB**: Para conectar o ESP32 ao computador.
- **Arduino IDE**: Para programar o ESP32.
- **Bibliotecas necessárias**: `WiFi`, `WebServer`, `ESPmDNS` (inclusas no pacote do ESP32).

## Estrutura do Projeto

O projeto é dividido em duas partes principais:

1. **Código do ESP32 (arquivo `.ino`)**:
   - Conecta-se a uma rede Wi-Fi existente.
   - Cria um servidor web com endpoints para acender e apagar o LED.
   - Serve uma página HTML para a interface de controle.

2. **Página HTML**:
   - Fornecida no arquivo `index.h` incluído no projeto.

## Instalação

### 1. Configuração do Ambiente

Certifique-se de que você tem o Arduino IDE instalado e o pacote ESP32 configurado. Se você ainda não configurou o ESP32 no Arduino IDE, siga [estas instruções](https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html).

### 2. Carregar o Código no ESP32

1. Abra o Arduino IDE e crie um novo sketch.
2. Cole o código do ESP32 (disponível no arquivo `server.ino`).
3. Conecte o ESP32 ao computador via cabo USB.
4. Selecione a placa e a porta corretas no menu **Ferramentas**.
5. Clique em **Upload** para carregar o código no ESP32.

### 3. Conectar-se ao ESP32

1. Certifique-se de que o ESP32 está conectado à rede Wi-Fi especificada no código.
2. Abra um navegador web e acesse o endereço IP do ESP32 (exibido no Monitor Serial após a conexão bem-sucedida).

## Uso

Após conectar o ESP32 à rede Wi-Fi, abra um navegador web e acesse o endereço IP do ESP32. Você verá uma página web com botões para acender e apagar o LED. Clique nos botões para controlar o LED.
