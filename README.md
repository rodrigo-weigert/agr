# Instruções
Este lab utiliza um filesystem próprio. Substitua a pasta `$NETKIT_HOME/fs` pela encontrada no arquivo `NETKIT_FILESYSTEM.tar.gz` deste repositório. Faça backup de seu filesystem antigo se julgar necessário.

O arquivo `NETKIT_FILESYSTEM.tar.gz` está dividido em partes devido ao limite do GitHub. Para extraí-lo, use `cat NETKIT_FILESYSTEM.tar.gz.* | tar xzvf -`.

Para uma inicialização mais rápida do lab, alterar o valor `MAX_SIMULTANEOUS_VMS` em `$NETKIT_HOME/netkit.conf` para `0`.

Para uma finalização segura e rápida do lab, use `lhalt -q;lclean` dentro do diretório raiz do lab. Se o sistema operacional hospedeiro é de 64 bits e o comando `lhalt` não consegue finalizar as máquinas, tente instalar a biblioteca `libncurses5:i386`.

# Informações Úteis

* IP interno do servidor da empresa: `10.0.0.2`
* IP externo da empresa: `200.155.29.17`
	* Servidor pode ser acessado tanto internamente como externamente (`WWW`) com `maxima.com.br` ou `www.maxima.com.br`
	* Servidor pode ser acessado via SSH. Senha do usuário `root`: `root`.
* IP da máquina `WWW` (simula acesso à internet a partir da empresa): `200.155.29.1`
	* `WWW` roda apache e oferece uma página HTML para teste.
	* Pode ser acessado dos computadores da empresa também com `www.website.com` ou `website.com`.
* Senha do usuário `root` no MySQL do servidor: `maxima`
* O _osCommerce_ está instalado no servidor e pronto para ser configurado. Basta acessar `maxima.com.br/install` (ou `127.0.0.1/install`, se estiver no próprio servidor)
