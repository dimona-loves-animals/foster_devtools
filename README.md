# Foster Cloud

## Initialize

Create `.env` file from `.env.example`.

> Make sure to create unique SECRET_KEY

Start using:

    docker-compose up -d

use `docker ps` to find the `foster_devtools_web` CONTAINER ID.

### Database migration (at first run, or after updates)

    docker exec -it container_id python manage.py migrate

### Create super-admin user

    docker exec -it container_id python manage.py createsuperuser


