
# Create a new project directory

    mkdir owncloud-docker-server

    cd owncloud-docker-server
# clone project

    git clone https://github.com/fcessi/owncloud-docker.git .

# Create the environment configuration file

cat << EOF > .env  
OWNCLOUD_VERSION=10.3  
OWNCLOUD_DOMAIN=localhost  
ADMIN_USERNAME=admin  
ADMIN_PASSWORD=admin  
HTTP_PORT=8080  
EOF

# Build and start the container

docker-compose up -d
