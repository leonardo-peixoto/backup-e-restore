#!/bin/bash


#senha PGADMIN
export PGPASSWORD="123123"

#código
pg_dump -U postgres -h localhost -O -o -b -F c faculdade > /home/leonardo/Documentos/leonardo.backup


#mensagem
echo echo "backup realizado!!!."
exit 






#!/bin/bash

#senha PGADMIN
export PGPASSWORD="123123"

#código
pg_restore -U postgres -h localhost -d faculdade2 /home/leonardo/Documentos/leonardo.backup


#mensagem
echo echo "Seu backup foi restaurado com sucesso."
exit 
