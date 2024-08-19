# timearmor-hackathon-2024-compose-dev
Dev Environment for Time Armor Hackathon 2024

# Installation
- Clone this repo using `git clone https://github.com/bilwit/timearmor-hackathon-2024-compose-dev.git`
- Within the `timearmor-hackathon-2024-compose-dev` folder, run `docker compose up -d`

# Usage/Setting up the Dev Environment
- Open Visual Studio Code and with the Docker extension, attach the workspace to the running `timearmor-hackathon-2024-server` container
- Open the folder `/var/www/html/`
- Copy the pre-configured project boilerplate using `git clone https://github.com/bilwit/timearmor-hackathon-2024.git`
- Install project dependencies using `cd timearmor-hackathon-2024; npm ci; cd client; npm ci; cd ..`