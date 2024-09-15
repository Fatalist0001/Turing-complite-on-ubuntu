##  Установка и запуск Turing Complete на Ubuntu

Этот файл README содержит инструкции по установке и запуску игры Turing Complete на Ubuntu.

### 1. Обновление системы
* Откройте терминал.
* Введите следующие команды:
    ```bash
    sudo apt update
    sudo apt upgrade
    ```

### 2. Установка Wine
* Добавьте поддержку архитектуры i386:
    ```bash
    sudo dpkg --add-architecture i386
    ```
* Установите Wine:
    ```bash
    sudo apt -y install wine
    ```

### 3. Настройка Wine
* Запустите конфигуратор Wine:
    ```bash
    winecfg
    ```
* В настройках Wine выберите версию Windows 10/11.

### 4. Запуск игры
* Найдите директорию с исполняемым файлом Turing Complete.exe.
* Откройте терминал в этой директории.
* Запустите игру с помощью команды:
   ```bash
    wine 'Turing Complete.exe'
   ```

### 5. Удаление Wine
* Если вам больше не нужна Wine, вы можете удалить её с помощью следующих команд:
    ```bash
    sudo apt purge wine
    rm -r ~/.wine
    rm -r ~/.config/menus/applications-merged/wine*
    rm -r ~/.local/share/applications/wine
    rm -r ~/.local/share/desktop-directories/wine*
    rm -r ~/.local/share/icons/????_*.xpm
    ```

Важно:
* Убедитесь, что у вас есть лицензионная копия игры Turing Complete.
* Этот файл README предназначен для информационных целей и не гарантирует работоспособность игры. 
* В случае возникновения проблем обратитесь к документации Wine

# English

## Installing and running Turing Complete on Ubuntu

This README file contains instructions on how to install and run the game Turing Complete on Ubuntu.

### 1. Updating the system
* Open a terminal.
* Enter the following commands:
    ```bash
    sudo apt update
    sudo apt upgrade
    ```

### 2. Installing Wine
* Add support for the i386 architecture:
    ```bash
    sudo dpkg --add-architecture i386
    ```
* Install Wine:
    ```bash
    sudo apt -y install wine
    ```
### 3. Configuring Wine
* Launch the Wine configuration tool:
    ```bash
    winecfg
    ```
* In the Wine settings, select the Windows 10/11 version.

### 4. Running the game
* Find the directory with the executable file Turing Complete.exe.
* Open a terminal in this directory.
* Run the game using the command:
    ```bash
    wine 'Turing Complete.exe'
    ```

### 5. Uninstalling Wine
* If you no longer need Wine, you can uninstall it using the following commands:
    ```bash
    sudo apt purge wine
    rm -r ~/.wine
    rm -r ~/.config/menus/applications-merged/wine*
    rm -r ~/.local/share/applications/wine
    rm -r ~/.local/share/desktop-directories/wine*
    rm -r ~/.local/share/icons/????_*.xpm
    ```

Important:
* Make sure you have a licensed copy of the Turing Complete game.
* This README file is for informational purposes only and does not guarantee the game's functionality. 
* If you encounter any problems, refer to the Wine documentation.
