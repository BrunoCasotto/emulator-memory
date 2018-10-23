# emulator-memory
Esse script tem o intuito de utilizar o gdrive (https://github.com/prasmussen/gdrive) para salvar/recuperar status de emuladores no ubuntu.

# Passos para configurar:
Baixar o arquivo do gdocs
``` 
cd ~
wget https://docs.google.com/uc?id=0B3X9GlR6EmbnWksyTEtCM0VfaFE&export=download
```

alterar o nome (conforme o arquivo que foi baixado)
```mv uc\?id\=0B3X9GlR6EmbnWksyTEtCM0VfaFE gdrive```

dar permissao para executar
```chmod +x gdrive```

instalar o gdrive local
```sudo install gdrive /usr/local/bin/gdrive```

executar primeiro comando
```gdrive list```
Nesse momento um link aparecera no terminal, abra o navegador com ele e de permissao para o aplicativo na sua conta gmail.

# Utilizando o emulator-memory
```git clone https://github.com/BrunoCasotto/emulator-memory.git```

entrar na pasta
``cd emulator-memory``
instalar
``` sudo install memory /usr/local/bin/emulator-memory```

* para salvar o status do seu zsnes execute o comando:
``` emulator-memory save ```

* para recuperar o status do seu zsnes execute o comando:
``` emulator-memory restore ```

* para salvar/recuperar o status de outro emuladores que tenham pastas escondidas na home do sistema utilize
``` emulator-memory [nome_do_emularos] [restore/save] ```

Obs: Quando o comando restore e executado uma pasta .[nome_do_emulador].bkp e criada no mesmo folder onde a nova versao foi atualizada, em caso de engano e so recuperar ela de la.