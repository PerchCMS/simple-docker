# simple-docker

A simple docker-compose setup for Perch or Runway

## Getting Started

First install Docker, if you're on a mac this is simple with the brilliant docker installer https://docs.docker.com/docker-for-mac/install/

Now once you have Docker installed check it's available in your terminal by running:

    docker --version

You should get something like:

    Docker version 17.06.0-ce, build 02c1d87

If that's the case you're now ready to run docker.

## Up and running

Now provision and start up the Docker Compose environment by running in your terminal:

    docker-compose up

This will pull the latest php & mysql docker images and get them up and running.

You may get Apache complain with "Could not reliably determine the server's fully qualified domain name, using 172.18.0.3. Set the 'ServerName' directive globally to suppress this message" but that's just because the php docker recipe doesn't automatically assign a Server Name, nothing to worry about for now.

Ok, now point your browser to => http://0.0.0.0

You should see the PHP Info page which is proof it's serving anything in this repo's /www directory, place your files in there and your ready to roll.

Enjoy.
