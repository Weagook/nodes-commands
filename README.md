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

Проверка логов

    journalctl -u subspaced -f -o cat
