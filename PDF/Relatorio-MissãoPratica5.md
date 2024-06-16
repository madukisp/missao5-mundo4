<style>
.custom-font {
  font-family: 'Arial', sans-serif; 
  font-size: 16px;
}
</style>

<div class="custom-font">

<p align="center">
<img src="https://i.pinimg.com/originals/1a/21/6f/1a216fb0afdce66e7ffd9c9dbfce393b.jpg" alt="Logo do Projeto" width="200"/>
</p>
<h2 align="center">RPG0027  - Vamos interligar as coisas com a nuvem</h2>
<h3 align="center">Missão Prática | Nível 5 | Mundo 4</h3>

* **Aluna:** Amanda Duque Kawauchi
* **Matrícula:** 202209170254
* **Campus:** Morumbi
* **Curso:** Desenvolvimento Full-Stack
* **Disciplina:** RPG0027  - Vamos interligar as coisas com a nuvem
* **Turma:** 2024.1
* **Semestre Letivo:** 4º Semestre
* **Repositório GitHub:** [Link do Repositório GitHub](https://github.com/madukisp/missao5-mundo4)

## Objetivo da Prática

Este projeto tem como objetivo desenvolver uma aplicação Node.js que se integra com o Azure IoT Hub para coletar e visualizar dados de dispositivos IoT. O intuito é aplicar conceitos de computação em nuvem e Internet das Coisas (IoT) para criar uma solução de visualização de dados.

## Análise e Conclusão

### Funcionalidades Implementadas

A aplicação implementa uma estrutura para conectar, enviar e visualizar dados de dispositivos IoT utilizando o Azure IoT Hub. As funcionalidades incluem:

- **Conexão com IoT Hub**: Configuração e conexão segura com o Azure IoT Hub.
- **Leitura de Dados**: Captura e processamento de dados enviados pelos dispositivos.
- **Visualização de Dados**: Interface web para visualização dos dados coletados em tempo real.

### Navegação e Interatividade

Utilizamos o Visual Studio Code para o desenvolvimento do projeto, incluindo a configuração do ambiente, instalação de dependências e execução da aplicação. A aplicação se comunica com o Azure IoT Hub para receber dados de dispositivos IoT e exibi-los em uma interface web.

### Desafios Encontrados

Alguns dos desafios enfrentados incluíram a configuração inicial do ambiente Azure, a definição das variáveis de ambiente e a integração com o Azure IoT Hub. Garantir a correta autenticação e segurança na comunicação com o IoT Hub foi crucial para o sucesso do projeto.

## Comandos Utilizados

### Configuração do Ambiente

```bash
# Definir variáveis de ambiente para conexão com o IoT Hub
export IotHubConnectionString="HostName=microatividade1.azure-devices.net;SharedAccessKeyName=service;SharedAccessKey=HLK+wk46T5eJ7NbFP9xlqITNy/7kF1gbeAIoTIAlWG8="
export EventHubConsumerGroup="missao"

# Clonar o repositório do projeto
git clone <URL-DO-SEU-REPOSITÓRIO>
cd web-apps-node-iot-hub-data-visualization

# Instalar dependências
npm install

# Iniciar o projeto
npm start
```

### Consultar Dados

```bash
# Executar consultas para verificar os dados recebidos do IoT Hub
az iot hub monitor-events --hub-name microatividade1 --device-id meu-dispositivo --consumer-group $EventHubConsumerGroup
```

### Configuração no Visual Studio Code

1. Abra o projeto no Visual Studio Code.
2. Navegue até o diretório `scripts` e edite os arquivos `iot-hub-connection-string.js` e `event-hub-reader.js` para garantir que as variáveis de conexão estejam corretas.
3. Utilize o terminal integrado do Visual Studio Code para executar os comandos de configuração e inicialização.

## Conclusão

O desenvolvimento deste projeto destacou a importância de uma configuração correta e da utilização de ferramentas adequadas como o Azure IoT Hub e o Visual Studio Code. Com uma aplicação robusta e funcional, foi possível explorar as capacidades de comunicação e visualização de dados em tempo real, proporcionando uma experiência prática e enriquecedora no campo da Internet das Coisas.

</div>
```