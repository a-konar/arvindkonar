
# Make sure you are under loki folder

# Run Loki as a single binary
docker-compose -f docker-compose-single-binary.yaml up -d

# Run Loki as a simple scalable deployment
docker-compose -f docker-compose-simple-scalable.yaml up -d

# Run nginx app
docker run --name nginx_front -d -p 8080:80 nginx:latest

# Reference

https://gist.github.com/wardbekker/6abde118f530a725e60acb5adb04508a

