# ProvaPROG

### Funcionalidades do Sistema

1. **Inicialização do Sistema**: O sistema configura os pinos dos LEDs e do botão. Os LEDs são configurados como `OUTPUT`, enquanto o botão é configurado como `INPUT`.

2. **Verificação do Estado do Botão**: O sistema lê constantemente o estado do botão para determinar se ele está pressionado ou não:

   - **Pressionado**: Quando o botão é pressionado, o sistema realiza uma ação específica, como acender um LED ou enviar uma requisição HTTP.
   - **Não Pressionado**: O sistema entra em um modo de espera, aguardando a próxima interação com o botão.

3. **Acender LEDs**:
   - **LED Verde**: Indica um estado de "Aguardando Ação" ou "Ação Confirmada". Ação realizada quando o botão é pressionado.
   - **LED Vermelho**: Indica um estado de "Erro" ou "Alerta". Pode ser ativado em resposta a um erro ou problema.
   - **LED Amarelo**: Pode ser usado para indicar estado de "Aguardando" ou "Processando".

4. **Desligar LEDs**: Após um tempo determinado (por exemplo, 5 segundos), o LED verde é desligado, indicando o fim da ação.

5. **Modo de Espera**: Quando não há interação (botão não pressionado), o sistema permanece em espera, pronto para relatar uma nova ação quando o botão for pressionado.
