# aplicando_P2P_Para_Compartilhamento_De_Arquivos

O código implementa uma aplicação P2P para compartilhamento de arquivos. Ele possui dois
modos principais:

1. Modo Servidor: o peer atua como servidor e disponibiliza arquivos que estão em uma pasta
chamada 'compartilhado'. Quando outro peer solicita a lista de arquivos ou um download, o servidor
responde diretamente.

2. Modo Cliente: o peer atua como cliente e pode se conectar a outro peer para listar os arquivos
disponíveis e fazer o download do arquivo desejado.

O código utiliza sockets TCP para estabelecer comunicação entre os peers. As funções principais
são:
- start_server(): inicia o servidor e aguarda conexões.
- handle_client(): processa pedidos de clientes (listar arquivos ou enviar arquivos).
- list_files(): conecta a outro peer para listar arquivos disponíveis.
- download_file(): baixa um arquivo específico de outro peer.

O usuário pode escolher no menu inicial se deseja atuar como servidor ou cliente.


