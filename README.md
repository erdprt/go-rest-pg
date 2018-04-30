About postgres:
Enter docker:                   docker exec -it $id /bin/bash
                                docker exec -it rest-pg-db /bin/bash
Enter psql for database:        docker exec -it $id psql -d rest-pg -U admin
                                docker exec -it rest-pg-db psql -d rest-pg -p 5432 -h 127.0.0.1 -U admin

PGDATA directory                PGDATA: /var/lib/postgresql/data 

Having persistent data for postgresql
    Create a volume:
        docker volume create --name postgresql-volume -d local
    Run:
        docker-compose -f docker-compose-pers.yml up -d --build 