# Instruções
Este lab utiliza um filesystem próprio. Substitua a pasta `$NETKIT_HOME/fs` pela encontrada no arquivo `NETKIT_FILESYSTEM.tar.gz` deste repositório. Faça backup de seu filesystem antigo se julgar necessário.

Para uma inicialização mais rápida do lab, alterar o valor `MAX_SIMULTANEOUS_VMS` em `$NETKIT_HOME/netkit.conf` para `0`.

Para uma finalização segura e rápida do lab, use `lhalt -q;lclean` dentro do diretório raiz do lab. Se o sistema operacional hospedeiro é de 64 bits e o comando `lhalt` não consegue finalizar as máquinas, tente instalar a biblioteca `libncurses5:i386`.
