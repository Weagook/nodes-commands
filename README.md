# nodes-commands

### Shardeum

Проверка состояния ноды

    ~/.shardeum/shell.sh
    operator-cli status
    
Удалить ноду

    cd ~/.shardeum
    ./cleanup.sh
    cd ~/
    rm -rf .shardeum
    rm installer.sh
    
Проверка активных докеров

    docker ps
    
### Subspaced


    
## Установка

Скрипт для быстрой установки

    wget -O subspace.sh https://api.nodes.guru/subspace.sh && chmod +x subspace.sh && ./subspace.sh

[Гайд на создание кошелька](https://docs.subspace.network/docs/protocol/wallets/subwallet/)

Проверка логов

    journalctl -u subspaced -f -o cat
    
Рестарт ноды

    sudo systemctl restart subspaced
    
Удаление ноды

    sudo systemctl stop subspaced
    sudo systemctl disable subspaced
    rm -rf ~/.local/share/subspace*
    rm -rf /etc/systemd/system/subspace*
    rm -rf /usr/local/bin/subspace*
