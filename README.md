# demo-restapi

## Command

- Run Postgres

`docker run --rm   --name pg-docker -e POSTGRES_PASSWORD=docker -d -p 5432:5432 -v $HOME/docker/volumes/postgres:/var/lib/postgresql/data  postgres`

## Data Insert

    CREATE TABLE IF NOT EXISTS public.user (
      id SERIAL NOT NULL,
      name varchar(20) NOT NULL DEFAULT '',
      hobby varchar(20) NOT NULL DEFAULT '',
      PRIMARY KEY (id)
    )

    INSERT INTO public.user(id, name, hobby) VALUES(1, 'george', 'basketball');
    INSERT INTO public.user(id, name, hobby) VALUES(2, 'yusuke', 'guitar');

## Reference

- [Postgres](https://hackernoon.com/dont-install-postgres-docker-pull-postgres-bee20e200198)
- [Spring Boot](https://qiita.com/akkino_D-En/items/574ccdc057849e0e22ce)
- [Conneciton](https://dev.classmethod.jp/server-side/java/using_spring_boot_2/)

