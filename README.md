Descrição do funcionamento e uso para reproduzir:

Vamos aprender como desenvolver um gráfico de ECG em plataforma IoT. Para isso, vamos conectar o sensor de ECG AD8232 ao ESP32 e criar um sinal de ECG conectando os eletrodos ao corpo. 
  O método utilizado para desenvolver o projeto envolve as seguintes etapas: Inicialmente, o ambiente de desenvolvimento será configurado, o que inclui a instalação do Arduino para programar a placa ESP32. Em seguida, será feita a montagem dos componentes físicos do circuito, o sensor de ECG AD8232 será conectado à placa ESP32 e a outros dispositivos necessários, como a protoboard, utilizando fios de conexão conforme especificado na descrição de materiais.
	Após a montagem física, será realizada a programação da placa ESP32 utilizando Arduino. Este código será projetado para ler os dados do sensor de ECG AD8232, processá-los e enviá-los para a plataforma de nuvem. Será utilizado o protocolo MQTT para a comunicação com o Broker MQTT na nuvem. Com a ajuda dos parâmetros do Ubidots, Chave de API, utilizando a IDE Arduino, o gráfico de ECG será enviado para a nuvem utilizando um Broker MQTT.
	Uma vez configurada a plataforma de nuvem, o Broker MQTT será implementado para receber, rotear e distribuir os dados do sensor de ECG AD8232 enviados pela placa ESP32.
	Após a conclusão da implementação, testes extensivos serão realizados para verificar o funcionamento correto do sistema. Isso incluiu testes de comunicação entre o sensor de ECG AD8232, a placa ESP32 e o Broker MQTT, bem como a validação da transmissão e recebimento corretos de dados pela plataforma de nuvem. 
	Com o sistema funcionando conforme o esperado, o seu desempenho será avaliado para garantir a precisão e confiabilidade do monitoramento da frequência cardíaca,  assegurando uma implementação bem-sucedida e resultados confiáveis.

Modelo de montagem:

![image](https://github.com/mayaramoliveira/ESP32_AD8232/assets/159947412/5d6cf12e-8e25-40f2-b606-76b59432d9a7)

Componentes utilizados:

- Placa ESP32	 
- Sensor de ECG AD8232  
- Cabo de dados micro USB 5V	 
- ProtoBoard

Interfaces:
- Ubidots: Para publicar os dados na nuvem IoT, precisamos de alguma plataforma IoT e Ubidots é uma dessas plataformas. Ubidots oferece uma plataforma para desenvolvedores que permite capturar facilmente dados de sensores e transformá-los em informações acionáveis. A plataforma Ubidots pode enviar dados para a nuvem a partir de qualquer dispositivo habilitado para Internet. (https://ubidots.com/stem/)

  ![image](https://github.com/mayaramoliveira/ESP32_AD8232/assets/159947412/a115588c-d369-4d44-81ec-9b372a65726d)

- Arduino IDE: Para realizar a programação da placa ESP32, utiliza-se a IDE Arduino. O código será projetado para ler os dados do sensor de ECG AD8232, processá-los e enviá-los para a plataforma de nuvem. (https://www.arduino.cc/en/software)
  
![image](https://github.com/mayaramoliveira/ESP32_AD8232/assets/159947412/ee360e50-65c0-4356-a6bc-7cf85393b02f)
