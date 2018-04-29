About postgres:
Enter docker:                   exec -it $id /bin/bash
                                exec -it rest-pg-db /bin/bash
Enter psql for database:        docker exec -it $id psql -d rest-pg -U admin
                                docker exec -it rest-pg-db psql -d rest-pg -p 5432 -h 127.0.0.1 -U admin

PGDATA directory                PGDATA: /var/lib/postgresql/data 