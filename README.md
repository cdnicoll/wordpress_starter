# Starter for Wordpress

## Setup
```
# Init docker
docker-compose up -d

# Bring bash up inside docker
docker-compose exec wordpress bash
```

## Teardown
```
# Stop and Remove Containers, Networks, and Volumes
docker-compose down -v

# Remove Unused Docker Objects (Optional)
docker system prune -a --volumes

# 
```

## Download Wordpress (optional)
```
cd wordpress
curl -O https://wordpress.org/latest.tar.gz
tar -xzf latest.tar.gz --strip-components=1
rm latest.tar.gz
cd ..
```

##  Access Your WordPress Site and Complete Setup
Open your web browser and go to http://localhost:8000. You should see the WordPress setup page. Follow the on-screen instructions to complete the WordPress installation.

## Access phpMyAdmin (Optional)
Open your web browser and go to http://localhost:8080. Log in with the database root credentials (root / rootpass) to manage your database.