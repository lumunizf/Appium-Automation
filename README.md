# Appium-Automation

## Exercícios do curso:

 - [x] :calling: *"Testes Funcionais de aplicações Android com Appium"*


## Pré-Requisitos

 * Java instalado e configurado.
 * Eclipse IDE instalado.
 * Android Studio e SDK Tools instalado e configurado.
 * Emulador do Android instalado.
 * Appium Desktop instalado e configurado.
 

## Configuração do ambiente de teste (Windows 10)

### 1. **Instalação do Java**

- Download do instalador do [Java JDK 8](http://www.oracle.com/technetwork/pt/java/javase/downloads)
- Aceitar a licença clicando em "Accept License Agreement".
- Clicar no link para download referente ao seu sistema operacional (Windows x64).
- Após o download, executar a instalação (*next, next, finish*).


### 2. **Configuração das variáveis de ambiente do Java**

- Adicionar *JAVA_HOME* nas variáveis de ambiente:

    * Meu Computador > Botão direito: Propriedades > Configurações avançadas do sistema;
    * Propriedades do sistema: Aba 'Avançado' > Botão "Variáveis do ambiente";
    * Na área "Variáveis do sistema", clicar no botão 'Novo...';
    * Na janela "Nova variável de sistema", preencher o campo 'Nome da variável' com *JAVA_HOME* e o campo 'Valor da variável' com o caminho do diretório onde o Java foi instalado.

- Atualizar o *PATH* das variáveis de ambiente:

    * Ainda na área "Variáveis do sistema", selecionar a variável "Path" > botão Editar.
    * Acrescentar ao final das configurações > *;%JAVA_HOME%\bin* > botão OK.

- Validar a configuração das variáveis de ambiente

    * Acessar o prompt de comando e digitar:

```
java -version
```

> O sistema deve apresentar a versão do Java instalada.

- Ainda no prompt de comando, digitar:

```
javac -version
```

> O sistema deve apresentar a versão do compilador Java instalada.


### 3. **Instalação do Eclipse IDE**

- Download do [Eclipse IDE](http://www.eclipse.org/downloads/eclipse-packages/)
- Selecionar a opção "Eclipse IDE for Java EE Developers" referente ao seu sistema operacional (Windows x64).
- Descompactar e iniciar o executável.


### 4. **Instalação e configuração do Android Studio**

- Download do [Android Studio](https://developer.android.com/studio/index.html?hl=pt-br)
- Após o download, executar a instalação (*next, next, finish*).
- Instalar as ferramentas abaixo pelo Android Studio > Configure > SDK Manager:
    * **Aba SDK Platforms**: Android 6.0 (Marshmallow) | Android 7.0 (Nougat);
    * **Aba SDK Tools**: Android Emulator | Android SDK Build-Tools | Android SDK Platform-Tools | Android SDK Tools
- Clicar no botão OK para que o Android Studio baixe ou atualize os componentes marcados.

- :warning: **DICA!** Antes de clicar no botão OK, copiar o caminho do diretório que é apresentado no campo *"Android SDK Location"*.


### 5. **Configuração das variáveis de ambiente do Android Studio**

- Adicionar *ANDROID_HOME* nas variáveis de ambiente:

    * Meu Computador > Botão direito: Propriedades > Configurações avançadas do sistema;

    * Propriedades do sistema: Aba 'Avançado' > Botão "Variáveis do ambiente";

    * Na área "Variáveis do sistema", clicar no botão 'Novo...';

    * Na janela "Nova variável de sistema", preencher o campo 'Nome da variável' com *ANDROID_HOME* e o campo 'Valor da variável' com o caminho do diretório copiado do campo *"Android SDK Location"* (:warning: *vide dica do item 5*).

- Atualizar o *PATH* das variáveis de ambiente:

    * Ainda na área "Variáveis do sistema", selecionar a variável "Path" > botão Editar.

    * Acrescentar ao final das configurações > *;%ANDROID_HOME%\tools;%ANDROID_HOME%\tools\bin;%ANDROID_HOME%\platform-tools* > botão OK.

- Validar a configuração das variáveis de ambiente do Android Studio

    * Acessar o prompt de comando e digitar os seguintes comandos:

```
adb
```

```
emulator
```

```
uiautomatorviewer
```

> O sistema deve reconhecer estes três comandos.


### 6. **Instalação e configuração do Emulador do Android**

- Criar um novo projeto no Android Studio:

    * Seguir com as informações padrão até chegar na tela pós criação do projeto.
    * Na tela "My Application" > aba 'MainActivity.java' > clicar no botão 'AVD Manager'.
    * Na tela "Android Virtual Device Manager" > Clicar no botão 'Create Virtual Device'.
    * Selecionar as opções 'Phone', 'Nexus 5X' > clicar no botão 'Next';
    * Selecionar a versão 'Nougat' (Android 7.0) > clicar no botão 'Next' > botão 'Finish'.
    
- Inicializar o emulador:

    * Selecionar o emulador criado e clicar no botão 'Launch this AVD in the emulator'.

- :warning: **DICA!** Existe uma forma mais prática de abrir o emulador sem consumir tantos recursos da máquina:

    * No prompt de comando acessar o seguinte diretório:

```
cd %ANDROID_HOME%\tools
```

- Digitar o comando abaixo para apresentar o nome correto do emulador cadastrado:

```
emulator -list-avds
```

- Em seguida, digitar o comando:

```
emulator @Nexus_5X_API_24
```

> O emulador deverá ser iniciado, consumindo menos recursos da máquina. :simple_smile:


### 7. **Instalação e configuração do Appium**

- Download do [Appium Desktop](https://github.com/appium/appium-desktop/releases) - [Versão 1.3.2]
- Clicar no link para download referente ao seu sistema operacional.
- Após o download, executar a instalação (*next, next, finish*).
- Validar que a versão do Servidor é a 1.7.2.
- Inicializar o Servidor clicando no botão 'Start Server v1.7.2'.


# License

MIT License © Luciana Muniz Freire.