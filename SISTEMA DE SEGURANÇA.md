SISTEMA DE SEGURANÇA COM SENHA

DESCRIÇÃO:
O projeto de segurança com senha pode ser desenvolvido para controlar o acesso a algum dispositivo ou sistema, porta, cofre ou outro dispositivo.

OBJETIVO:
Proteger uma área, porta ou dispositivo controlando o acesso através uma verificação de senha enviada via Bluetooth. 

ORGANIZAÇÃO ELETRÔNICA:

  COMPONENTES NECESSÁRIOS:
- Arduino Uno R3: É uma placa microcontroladora do sistema;
- Módulo Bluetooth HC-05: Utilizado para uma conexão sem fio entre o arduíno e o dispositivo bluetooth;
- Sensor PIR; O sensor de presença é utilizado para detectar algum movimento;
- Sensor magnético MC-38; O sensor magnético é utilizado para monitorar abertura de portas e janelas;
- Buzzer ativo: Utilizado para emitir qualquer tipo de som;
- LED (vermelho e verde); O led vermelho é utilizado para alertar e o led verde para permitir um acesso;
- Resistores: Serve para controlar a corrente eletrica;
- Fios de conexão: Utilizado para conectar os componentes;
- Protoboard: Placa utilizada para montagem do sistema.

LÓGICA DO SISTEMA: 
O sistema é iniciado após identificar alguém se aproximando através do Sensor PIR ou intrusão através do Sensor Magnético.
Ao realizar a conexão via bluetooth, o sistema imprime no app e no monitor: “Sistema de segurança ativado.” 

Após detectar um movimento ou intrusão através dos sensores, o sistema imprime no app e no monitor: “Movimento detectado/ intrusão detectada”. 
O sistema aciona o led vermelho e o buzzer, e imprime outra mensagem para o app e no monitor: “Para continuar, digite sua senha:”			
Após o usuário inserir a senha, o sistema verifica a senha digitada e compara com a armazenada no código. 
Caso esteja correta, imprime no app “Sistema de segurança Desativado", apaga o led vermelho e para o som no buzzer. e imprime "Acesso Permitido. Seja bem-vindo (a)!”.
Acende o led verde e emite um som de permissão através do buzzer. 
Caso contrário, imprime no app e no monitor: "Senha incorreta. Tente novamente.”, o led vermelho apaga e o som no buzzer continua, até que,
o usuário se aproxime novamente do Sensor para digitar novamente a senha correta.
Após isso, o sistema volta ao seu estado de origem aguardando um novo movimento ou intrusão.
