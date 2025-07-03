# Treinador de Digitação (Touch Typing Trainer)

## Desenvolvedor

* **Nome:** Carlos Alberto
* **Contato (Telefone/WhatsApp):** +55 11 2615-2880

## Descrição

O Treinador de Digitação é uma aplicação desktop desenvolvida em Python com o objetivo de auxiliar usuários a aprimorar suas habilidades de digitação (touch typing). O programa foca no posicionamento correto dos dedos, precisão e velocidade, oferecendo exercícios em múltiplos idiomas e configurações de treino personalizáveis.

## Funcionalidades

* **Interface Gráfica do Usuário (GUI)**: Construída com PySimpleGUI para uma experiência limpa e amigável.
* **Suporte Multilíngue (na Aplicação)**:
    * A interface do usuário e as instruções estão disponíveis em **Português, Inglês e Italiano**.
    * O idioma pode ser selecionado na tela de boas-vindas.
* **Guia de Posicionamento das Mãos**:
    * Instruções textuais detalhadas para o posicionamento correto das mãos.
    * Diagramas em arte ASCII ilustrando:
        * Atribuições focadas dos dedos para a fileira QWERTY e a tecla à direita do 'P'.
        * Uma representação de um layout de teclado completo para contexto.
    * Orientação específica para o layout do teclado selecionado:
        * **Português**: Layout Brasileiro ABNT2.
        * **Inglês**: Layout QWERTY Americano Padrão.
        * **Italiano**: Layout QWERTY Italiano.
* **Modo de Treinamento**:
    * **Frases de Prática**: Digite frases fornecidas pela aplicação.
    * **Fontes das Frases**:
        * Utilize frases integradas à aplicação.
        * Carregue frases de um arquivo `.txt` externo fornecido pelo usuário.
    * **Comprimento da Frase (para frases integradas)**: Escolha entre frases Curtas, Longas ou Mistas. (Esta opção é ocultada ao usar frases de um arquivo).
    * **Feedback em Tempo Real**:
        * À medida que você digita, os caracteres na frase alvo exibida mudam de cor:
            * **Verde** para caracteres corretos.
            * **Vermelho** para caracteres incorretos.
    * **Limites de Tempo**:
        * **Modos Automáticos**:
            * Ritmo de Aprendizagem (tempo padrão baseado no comprimento da frase).
            * Tempo x2 (dobro do tempo do Ritmo de Aprendizagem).
            * Tempo x3 (triplo do tempo do Ritmo de Aprendizagem).
        * **Modo Manual**: Defina um limite de tempo customizado em segundos.
        * Um cronômetro exibe o tempo decorrido e o tempo máximo permitido durante o exercício.
* **Relatório de Desempenho**: Após cada exercício, um relatório detalhado inclui:
    * A frase alvo.
    * A frase que você digitou.
    * Comprimento da frase alvo.
    * Comprimento da sua frase digitada.
    * Contagem de erros (baseada na diferença entre o texto final digitado e o alvo).
    * **Total de Erros Cometidos**: Conta cada vez que um caractere incorreto foi digitado para uma posição, mesmo que corrigido posteriormente.
    * Percentual de precisão.
    * Tempo levado para completar o exercício.
    * Uma categoria qualitativa de desempenho (ex: "Velocidade Excelente!", "Foco na Precisão!", "Tempo Limite Excedido").
* **Arquivos de Texto Personalizados**:
    * **Carregar Frases**: Importe sua própria lista de frases de um arquivo `.txt` (uma frase por linha).
    * **Baixar Exemplo**: Baixe um arquivo `.txt` modelo para ver o formato requerido.
* **Interface Dinâmica**: A visibilidade de certos controles (como botões de operação de arquivo e opções de comprimento da frase) muda contextualmente com base nas suas seleções.

## Tecnologias Utilizadas

* **Python 3**
* **PySimpleGUI**: Para a interface gráfica.

## Configuração e Instalação

1.  **Certifique-se de que o Python 3 está instalado** no seu sistema.
2.  **Instale o PySimpleGUI**:
    ```bash
    pip install pysimplegui
    ```
3.  **Baixe o Código**:
    * Clone este repositório ou baixe o arquivo `TouchTypingTrainer.py` (ou o nome relevante do script Python).
4.  **Execute a Aplicação**:
    ```bash
    python TouchTypingTrainer.py
    ```

## Como Usar

1.  **Tela de Boas-vindas**:
    * Ao iniciar, você verá a tela de boas-vindas.
    * **Selecione seu idioma preferido** (Italiano, Inglês ou Português) usando os botões de rádio. Todo o texto da aplicação será atualizado.
2.  **Opções do Menu Principal**:
    * **Fonte das Frases**:
        * Escolha "Internas" para usar as frases predefinidas da aplicação.
        * Escolha "De Arquivo" para usar frases de um arquivo `.txt` que você fornecer.
    * **Comprimento da Frase** (Visível se a fonte "Internas" estiver selecionada):
        * Selecione "Curta", "Longa", ou "Mista".
    * **Operações de Arquivo** (Visível se a fonte "De Arquivo" estiver selecionada):
        * Clique em "Carregar Frases (.txt)" para procurar e selecionar seu arquivo de texto.
        * Clique em "Baixar Exemplo .txt" para salvar um arquivo modelo.
    * **Configurações de Tempo Limite**:
        * Escolha um limite de tempo automático (Ritmo de Aprendizagem, x2, x3) ou selecione "Manual" para inserir uma duração específica em segundos.
    * **Guia de Posicionamento das Mãos**:
        * Clique neste botão para abrir um pop-up com instruções detalhadas e diagramas ASCII sobre o posicionamento correto das mãos para o layout de teclado do idioma selecionado.
    * **Iniciar Treinamento**:
        * Clique para começar um exercício de digitação.
3.  **Janela de Treinamento**:
    * Uma frase será exibida para você digitar.
    * Um campo de entrada é fornecido para sua digitação.
    * Conforme você digita, os caracteres na frase alvo exibida mudarão de cor para verde (correto) ou vermelho (incorreto).
    * Um cronômetro mostrará seu tempo decorrido e o tempo máximo permitido.
    * Clique em "Enviar" (ou pressione Enter) ao terminar, ou se o tempo acabar, o exercício terminará automaticamente.
4.  **Janela de Relatório**:
    * Após cada exercício, um relatório mostrará suas métricas de desempenho.
5.  **Sair**: Clique no botão "Sair" para fechar a aplicação.

## Melhorias Futuras (Ideias Possíveis)

* Estatísticas mais detalhadas e acompanhamento do progresso ao longo do tempo.
* Contas de usuário para salvar preferências e progresso.
* Diferentes modos de treinamento (ex: exercícios de teclas específicas, lições personalizadas).
* Teclado visual que destaca as teclas a serem pressionadas.
* Feedback sonoro para erros ou conclusão.

## Contribuições

Contribuições são bem-vindas! Se você gostaria de contribuir, por favor, siga estes passos:
1.  Faça um Fork do repositório.
2.  Crie uma nova branch (`git checkout -b feature/SuaFuncionalidade`).
3.  Faça suas alterações.
4.  Faça o commit de suas alterações (`git commit -m 'Adiciona SuaFuncionalidade'`).
5.  Faça o push para a branch (`git push origin feature/SuaFuncionalidade`).
6.  Abra um Pull Request.

## Licença

MIT License

Copyright (c) 2025 Carlos Alberto

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
