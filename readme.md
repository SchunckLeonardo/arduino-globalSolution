## Problema de Saúde Abordado
A superlotação em hospitais e as longas filas de espera para atendimento são desafios significativos na área da saúde, impactando negativamente a eficiência e a qualidade dos serviços prestados.

## Visão Geral da Solução Proposta
Para enfrentar o problema da superlotação hospitalar e otimizar o processo de atendimento, desenvolvemos uma aplicação de Fila Virtual. Essa solução permite que os pacientes se coloquem na fila de espera remotamente e, quando o número deles está prestes a ser chamado, recebam uma notificação para que possam se dirigir ao local de atendimento.

### Funcionalidades Principais:
1. **Verificar Lotação do Hospital:**
   - Os usuários podem verificar a lotação do hospital antes de decidirem ir até o local.

2. **Chamar o Próximo da Fila:**
   - O sistema gera automaticamente o próximo número da fila, facilitando o chamado e atendimento dos pacientes.

3. **Verificar Status do Paciente:**
   - Adicionamos a funcionalidade de verificar o status do paciente na fila, fornecendo informações sobre a posição atual na espera.

4. **Ver a Hora Atual:**
   - Incluímos uma funcionalidade simples para visualizar a hora atual, proporcionando uma experiência mais completa aos usuários.

## Instruções de Configuração e Uso:

### Requisitos Prévios:
1. Certifique-se de ter uma instância do Node-RED em execução.
2. Garanta que o MQTT Broker esteja configurado e acessível.

### Configuração do Node-RED:
1. Importe o fluxo fornecido no arquivo `flow.json` para o seu ambiente Node-RED.

2. Conecte o bloco MQTT In ao seu broker MQTT. Certifique-se de configurar o tópico adequado para receber os valores.

3. Configure o bloco Trigger para fornecer a mensagem de boas-vindas ao iniciar o sistema. Ajuste o tempo de duração conforme necessário.

4. Configuração do Telegram:
   - Configure o bloco Telegram Sender com as credenciais do seu bot Telegram.
   - Ajuste o bloco Function 1 para definir as opções do teclado inline.

### Configuração Adicional:
1. Se necessário, ajuste os parâmetros do bloco Function 3 para personalizar a lógica de verificação de lotação, chamada do próximo da fila, etc.

2. Certifique-se de que as bibliotecas e dependências necessárias estejam instaladas no ambiente Node-RED.

### Uso do Bot Telegram:
1. Inicie o bot no Telegram digitando `/start` para receber a mensagem de boas-vindas.

2. Utilize os botões de comando disponíveis para verificar a lotação do hospital, chamar o próximo da fila, verificar a hora atual ou o status do paciente.

### Simulação do Projeto:
Acesse a [simulação do projeto no Wokwi](https://wokwi.com/projects/381738548110061569) para visualizar a interação com o bot e testar as funcionalidades disponíveis.

Essas instruções guiarão você na configuração e uso inicial do sistema de Fila Virtual. Personalize conforme necessário para atender às especificidades do seu ambiente e requisitos.
