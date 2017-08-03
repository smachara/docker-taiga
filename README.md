# Taiga with Events Setup

To use this container, as-is, simply clone this repo and startup Docker:

```bash
git clone https://github.com/smachara/docker-taiga.git mytaiga
cd mytaiga/

# Optional, but likely desired, update your configuration now
nano docker-compose.yml # Be sure to update the TAIGA_HOSTNAME
nano taiga-conf/conf.json
nano taiga-conf/local.py

# Startup docker containers
docker-compose  up -d

# Wait ~30 seconds. The taiga container will initialize your postgres database.

# Now open your web browser:
open http://localhost/

Once your container is running, use the default administrator account to login: username is admin, and the password is 123123.
