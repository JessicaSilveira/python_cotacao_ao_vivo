### **Título:** Bot Trader Simples: Seus primeiros passos no mundo da programação para trading

### **Descrição:**

Quer dar seus primeiros passos no mundo da programação para trading? Esse script te ajuda a conectar com o MetaTrader 5 e buscar informações em tempo real sobre seus ativos favoritos. É como ter um assistente pessoal te atualizando sobre as últimas movimentações do mercado!

### **Funcionalidades:**

* **Conexão com o MetaTrader 5:** Estabelece uma conexão com sua conta no MetaTrader 5.
* **Busca por símbolos:** Encontra os símbolos disponíveis para negociação em sua conta.
* **Cotações em tempo real:** Obtém informações atualizadas sobre o preço de um ativo específico.
* **Monitoramento contínuo:** Atualiza as informações a cada segundo, te mantendo informado sobre as últimas movimentações.

### **Como usar:**

1. **Instale as bibliotecas:** Certifique-se de ter o MetaTrader 5 instalado e configurado em sua máquina. Em seguida, instale a biblioteca `MetaTrader5` usando o comando `pip install MetaTrader5`.
2. **Execute o script:** Rode o script Python em seu ambiente de desenvolvimento.
3. **Configure os símbolos:** Altere o símbolo no código para acompanhar o ativo de sua preferência.

### **Tecnologias utilizadas:**

* **Python:** A linguagem que torna tudo possível! 
* **MetaTrader5:** Plataforma de negociação que fornece acesso aos dados de mercado.

### **Exemplo:**

```python
# ... (código anterior)

# Monitorar o ativo PETR4
simbolo = "PETR4"

while True:
    tick = mt5.symbol_info_tick(simbolo)
    print(f"O fechamento de {simbolo} é {tick.last}")
    print(f"O valor de compra de {simbolo} é {tick.ask}")
    print(f"O valor de venda de {simbolo} é {tick.bid}")
    print(f"=================================")
    time.sleep(1)
```
