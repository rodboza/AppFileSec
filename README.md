# AppFileSec
App para gerenciar arquivos com segurança

teste

APP para gerenciar arquivos com segurança

Eu preciso de um app que monitore uma ou mais pastas, com seus subpastas e que sempre quando um arquivo for alterado o mesmo deve realizar um backup em uma outra pasta assim configurada. Se a pasta de destino do backup não estiver disponível, acumular as alterações e enviar assim que possível

Importante que os arquivos do backup sejam gravados de forma criptografada

Seria interessante se esse app possibilitasse o controle de usuários e o compartilhamento de pastas/arquivos com os demais usuários cadastrados. 

Se possível esse app também poderia notificar o usuário informando que houve atualização e se o mesmo aceita receber as atualizações ou se ele gostaria apenas de visualizar o arquivo

Casos de teste
	Cadastrar 1 pasta 
		? Cadastrar uma pasta e verificar cadastros da pasta
	Cadastrar 10 pastas
		? Cadastrar 10 pastar e verificar se tem 10 pastas
	Monitorar um arquivo em uma pasta
		? Cadastrar uma pasta, criar um arquivo nela e verificar se foi sinalizado
	Monitorar dois arquivos em uma pasta
		? Cadastrar uma pasta, criar dois arquivos na mesma pasta e verificar se foi sinalizado
	Monitorar dois arquivos em pastas diferentes
		? Cadastrar duas pastas, criar um arquivo em cada pasta e verificar se foi sinalizado
	Monitorar arquivos em uma subpasta
		? Cadastrar uma pasta com sinalização de subpasta, criar um arquivo na subpasta e verificar se foi sinalizado
	Monitorar alteração de arquivo
		? Cadastrar uma pasta, criar um arquivo nessa pasta, verificar se foi sinalizado, realizar um backup (mock), verificar se ainda tem arquivo sinalizado, alterar o arquivo, verificar se foi sinalizado
	Cadastrar uma pasta de backup
		? Cadastrar uma pasta do tipo backup, verificar cadastro
	Simular indisponibilidade da pasta de backup
		? Cadastrar uma pasta, criar um arquivo nessa pasta, verificar se foi sinalizado, realizar um backup (mock induzido ao erro) , verificar se ainda tem arquivo sinalizado, verificar se tem arquivo pendente, realizar um backup (mock sem erro), verificar se ainda tem arquivo sinalizado, verificar se tem arquivo pendente
