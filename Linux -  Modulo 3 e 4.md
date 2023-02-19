# Linux - Primeiros Passos - Módulo 3: Conhecendo o Ambiente do Linux Mint

`Curso em v[ideo - Gustavo Guanabara. Link: [Linux [40 Horas] - Curso em Vídeo](https://www.cursoemvideo.com/curso/linux/)`

- Ferramenta Time shift => pode criar o timeshift para fazer o backup. É importante criar o timeshift antes de fazer grandes mudanças no sistema pois caso o sistema morra, você tem um backup com a última versão do sistema que você criou

### CRON - gerenciador de tarefas (*curiosidade minha*)

- O Cron é um comando do Linux que permite programar tarefas para serem executadas de maneira independente
- É um recurso de automação

# Linux - Primeiros Passos - Módulo 4: Instalação básica de programas no Linux

Há duas maneiras de fazer essa instalação, a primeira é pelo **Terminal** e a segunda é pela **Loja de aplicativos do Mint**

### Lojas de aplicativos do Mint

- No menu inicial do Mint tem o *Gerenciador de Aplicativos*, clicando nessa opção irá abrir a loja de aplicativos na qual você pode instalar os apps disponíveis (basta confirmar a primeira tela que aparece e colocar sua senha), tem menos apps do que o Synaptic

### Instalando pelo Terminal, pelo Synaptic e por pacote

- #### Synaptic
  
  - Tem vários repositórios que tem programas livres. Você poderá selecionar o pacote que você deseja instalar 
  
  - Basta procurar pelo *Synaptic* no menu do mint que irá abrir a tela e aí é procurar o app desejado, botão direito *Marcar para instalação*, clica duas vezes, seleciona marcar
  
  - Clica em *Aplicar* na parte superior do gerenciador pelo Synaptic

- #### Instalando por pacote (apt)
  
  - Ferramenta de manipulação de repositórios onde é possível baixar programas. Tem vários comandos que você pode usar (tem até a piada do apt moo)
  
  - Para ver todas as opções é só colocar no terminal *apt*
  
  - *Apt get* - dá mais detalhes de alguns comandos mais usados descrevendo o que eles fazem
  
  - Para instalar o pacote é colocar:
    
    - ```
      apt install nomeDoPacot
      
      //htop é um programa para ver como está a sua CPU
      apt install htop
      ```
  
  - Após isso irá aparecer para colocar a senha e o programa é instalado
  
  - ### Para desinstalar
    
    - ```
      apt remove nomedoPacote
      
      apt remove htop
      ```
    
    - Outra forma (para remover apps que você baixou direto da internet)
      
      - Pelo terminal, vai até a pasta que você baixou o programa e coloca?
      
      - ```
        sudo dpkg --remove nomeDoArquivoQueVoceBaixou
        
        Para remover manualment o visual studio code
        sudo dpkg --remove code
        ```
      
      -  
  
  - ### Para procurar outros pacotes
    
    - ```
      apt search NomeDoPacoteQueVoceQuerProcurar
      sudo apt install eclipse-jdt
      ```
    
    - 
  
  - d

- #### Instalando app da Microsoft (Visual Studio)
  
  - Primeiro: baixa o arquivo da internet (no mint é .deb porque é baseado em uma versão do Debian)
  
  - **Primeira forma**
    
    - Dois cliques no arquivo baixado e seguir o que é indicado pelo Linux
  
  - **Segunda forma**
    
    - No terminal, vai até a pasta que você baixou o arquivo e digita?
    
    - ```
      sudo dpkg --install nomeDoArquivo
      sudo dpkg --install code
      ```

- #### Para limpar o cachê
  
  - ```
    sudo apt clean
    sudo apt autoremove
    ```
  
  - 
