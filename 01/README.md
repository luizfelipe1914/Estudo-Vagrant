### GERENCIAMENTO DAS BOXES

O vagrant utiliza imagens(vagrant boxes) para criar as máquinas virtuais. Essas boxes são disponibilizadas através do vagrant cloud, um repositório público de boxes. Para criar uma VM é necessário ter a box disponível localmente. Abaixo, são apresentados os comandos de gerenciamento das boxes:

OBS.: As boxes baixadas ficam armazenadas localmente no diretório ~/.vagrant/boxes

1. Obtendo ajuda:

```sh
    vagrant box -h
    vagrant box <command> -h
```

2. Listar as boxes:
```sh
    vagrant box list
```

3. Adicionar um box remota:
```sh
    vagrant box add <box_remota>
```

4. Listar as boxes outdated:
    4.1. Verifica globalmente. Tanto as boxes disponíveis localmente, quanto as existentes no hypervisor:
        ```sh
            vagrant box outdated --global 
        ```
    4.2. Verifica se as boxes utilizadas no projeto estão outdated:
        ```sh
            vagrant box utdated 
        ```


1. Remover as boxes obsoletas/desatualizadas:
```sh
    vagrant box prune
```

6. Remover uma box:
```sh
    vagrant box remove <box_name>
```

