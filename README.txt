To build and start 

    cd elk
    docker-compose -f docker-compose.yml -f extensions/logspout/logspout-compose.yml build
    docker-compose -f docker-compose.yml -f extensions/logspout/logspout-compose.yml up -d

    cd music
    docker-compose build
    docker-compose up -d

    docker-compose up --scale app=3 -d
    docker-compose restart proxy