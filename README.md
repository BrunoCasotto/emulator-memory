# zsnes-memory
Esse script tem o intuito de utilizar o gdrive (https://github.com/prasmussen/gdrive) para salvar/recuperar status do emulador zsne.

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

# Utilizando o zsnes-memory
```git clone https://github.com/BrunoCasotto/zsnes-memory.git```

entrar na pasta
``cd zsnes-memory``
instalar
``` sudo install memory /usr/local/bin/zsnes-memory```

* para salvar o status do seu zsnes execute o comando:
``` zsnes-memory save ```

* para recuperar o status do seu zsnes execute o comando:
``` zsnes-memory restore ```

Obs: Quando o comando restore e executado uma pasta .zsnes.bkp e criada no mesmo folder onde a nova versao foi atualizada, em caso de engano e so recuperar ela de la.
