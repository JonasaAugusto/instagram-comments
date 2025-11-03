# Bot de Mensagens para Instagram (script.py)

## 💻 Descrição
Este script Python atua como um **bot de automação** para enviar mensagens repetitivas em duas conversas distintas do Instagram (ou qualquer outra aplicação de chat baseada em desktop/web que use coordenadas de tela fixas).

Ele foi projetado para simular um comportamento humano, alternando entre duas "sessões" de envio de mensagens com pausas naturais e preventivas. O script utiliza a biblioteca `pyautogui` para controle do mouse e teclado, e `keyboard` para captura de eventos.

## ✨ Funcionalidades
*   **Automação de Envio:** Envia mensagens automaticamente para dois alvos diferentes (definidos como "Sogra" e "Força" no código).
*   **Mensagens Personalizadas:** Possui listas de mensagens e emojis pré-definidas para cada tipo de alvo, gerando combinações aleatórias.
*   **Simulação Humana:** Inclui pausas aleatórias entre as mensagens e simulação de movimento de mouse para evitar detecção como bot.
*   **Captura de Coordenadas:** Permite ao usuário capturar as coordenadas exatas do campo de mensagem e do botão de envio na tela, tornando-o adaptável a diferentes resoluções e layouts de aplicativos.
*   **Execução Contínua:** Projetado para rodar por um longo período (padrão de 14 horas), alternando entre as duas sessões de envio.

## ⚙️ Requisitos
Para executar este script, você precisará:
1.  **Python 3.x** instalado.
2.  As bibliotecas `pyautogui`, `keyboard`, `pyperclip` e `time`.

### Instalação das Dependências
```bash
pip install pyautogui keyboard pyperclip
```

## 🚀 Como Usar

1.  **Prepare o Ambiente:**
    *   Abra o aplicativo de chat (ex: Instagram Web ou Desktop) e deixe as duas conversas (alvo 1 e alvo 2) visíveis e prontas para receber mensagens.

2.  **Execute o script:**
    ```bash
    python script.py
    ```

3.  **Calibre as Coordenadas:**
    *   O script solicitará que você mova o mouse para o campo de mensagem e o botão de envio de cada alvo.
    *   Siga as instruções na tela, pressionando a tecla indicada (`M` para campo de mensagem, `P` para botão de envio) para capturar as coordenadas.

4.  **Inicie a Execução:**
    *   Após a calibração, o script pedirá para pressionar `Enter` para iniciar o envio contínuo de mensagens.

5.  **Interrupção:**
    *   Para interromper a execução a qualquer momento, pressione `Ctrl+C` no terminal.

## ⚠️ Observações de Segurança
*   **Risco de Bloqueio:** O uso de automação em plataformas como o Instagram pode violar os Termos de Serviço e levar ao bloqueio temporário ou permanente da sua conta. Use por sua conta e risco.
*   **Dependência de Tela:** O script depende das coordenadas de tela. Se a janela do aplicativo de chat for movida, redimensionada ou coberta, o script pode falhar ou enviar mensagens para o local errado.
*   **Configuração:** As mensagens e emojis são codificados diretamente no script. Para personalizá-los, edite as listas `mensagens_sogra`, `mensagens_forca`, `emojis_sogra` e `emojis_forca`.
