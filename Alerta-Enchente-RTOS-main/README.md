Ficha de proposta de projeto

Nome do Aluno: Samuel Guedes Canário
Polo: Bom Jesus da Lapa
Data:  19/05/2025

Título do Projeto
Estação de Alerta de Enchente

Objetivo Geral
O sistema que representa uma estação de monitoramento de cheias. Os dados de nível da água nos rios e o volume de chuva serão simulados pelo joystick da placa BitDog Lab com o RP2040.
O sistema processa a informação do analógico do joystick as quais geram informações:
• Alertas visuais com LED RGB e matriz de LEDs
• Alertas sonoros com o buzzer
• Exibição em tempo real no display OLED
Todos os componentes são controlados por tarefas FreeRTOS que se comunicam entre si por meio de filas.
Descrição Funcional:
O sistema implementado tem 2 modos de operação:
Modo Normal: Exibe continuamente os valores de nível da água e volume de chuva. Sinalizações
sonoras são desativadas.
Modo Alerta: Ativado automaticamente quando: Nível da água ≥ 70% ou Volume de chuva ≥ 80%.
Neste modo: LED RGB indica o alerta (vermelho). O buzzer emite sinais sonoros. A matriz de LEDs exibir um ícone ou símbolo de perigo. O display mostra os dados com destaque ao status de alerta.

Uso dos Periféricos da BitDogLab
Potenciômetro do Joystick: Simula um sensor de nível que vai de 0 a 100% 
Botão B: da boot no sistema
Display OLED: é atualizado com o monitoramento e o estado (Modo de operação), quando o nível chega a 70% ativa imediatamente o estado de alerta (Enchente).
Matriz de LEDs: exibe um símbolo de agua enquanto está normal, para sinalizar a chuva. Quando chega a um nível alarmante, mostra um símbolo de enchente (transbordou).
LED RGB: Conforme o nível da agua sobe o led vai variando sua coloração, indo do verde (normal) ao vermelho(enchente). 
Buzzer: Quando o nível ultrapassa os 69% ele começa a emitir um sinal de alerta.
Links para acesso ao código e ao vídeo.
https://youtu.be/eEqawhUwWZs

