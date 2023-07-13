- com o comando VIM "nome do arquivo" e execute os seguntes comandos

#!/bin/bash

diretorio_log="/mnt/efs/Wesley_Sergio"

arquivo_log="log-a.txt"
veririficar_apache () {
	systemct1 is-active --quiet httpd
	return $?
}

verificar_apache
if [$? -eq 0 ]; then
	status="online"
	mensagem="o serviço está online."
else
	status="offline"
	mensagem="o serviço está offline."
fi

- logo em seguida saia o modo edição com o botão ESC e digite :wq para salvar e sair
- utiize o comando chmod para habilitar as permissões que o script precisar, e use ./"nome do arquivo"
