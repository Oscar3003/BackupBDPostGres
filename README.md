# BackupBDPostGres
ShellScript BackupPostGres

#SHELLSCRIPTPARABACKUPBDPOSTGRE

#!/bin/sh

#bkp_livraria.sh

#DATA
DATA='/bin/date+%Y-%m-%d'

#Nome do arquivo de BACKUP

#Arquivo salvo:

#/www/virtual/backup é uma pasta publica do apache.

#diretorio do BACKUP.
NOME="/www/virtual/backup/livraria.sh-$DATA.sql"

#Variaveis do POSTGRESQL
HOST="localhost"

USER="postgres"

PASSWORD="12345"

DATABASE="livraria.sh"

pg_dump -h $localhost -u $postgres -p $12345 $livraria.sh > $livraria.backup
