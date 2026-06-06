# Permissões aplicadas
## Ambiente utilizado
VM local 
## Utilizador e grupos
Resumo dos comandos
whoami - kleiton-da-rosa
id - uid=1000(kleiton-da-rosa) gid=1000(kleiton-da-rosa) groups=1000(kleiton-da-rosa),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users),111(lpadmin),114(lxd)
groups - kleiton-da-rosa adm cdrom sudo dip plugdev users lpadmin lxd
## Ficheiros criados
- publico.txt:
- restrito.txt:
- script.sh:
## Permissões aplicadas
| Ficheiro | Permissão | Justificação |
|---|---:|---|
| publico.txt | 644 |permite que o proprietário tenha permissões de leitura e escrita, enquanto os restantes utilizadores do sistema têm apenas permissão de leitura  |
| restrito.txt | 640 | limitar o acesso apenas ao proprietário e aos membros do grupo associado ao ficheiro, impedindo que outros utilizadores do sistema tenham qualquer acesso. |
| script.sh | u+x |  adiciona a permissão de execução (x) apenas ao proprietário (u - user) do ficheiro|
## Relação com o princípio do menor privilégio
As permissões aplicadas são mais seguras do que permissões totais para todos, pois seguem o
 princípio do menor privilégio. Desta forma, cada utilizador possui apenas os acessos necessários, 
reduzindo o risco de alterações indevidas, execução não autorizada de ficheiros e exposição de informações
 sensíveis, contribuindo para a segurança e integridade do sistema.

