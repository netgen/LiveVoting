#LiveVoting

##How to install?

    git clone https://github.com/netgen/LiveVoting.git
    cd LiveVoting
    mkdir src
    cd src
    mkdir Netgen
    cd Netgen
    git clone https://github.com/netgen/LiveVotingBundle.git
    cd ../../
    # move to production mode
    composer install --no-dev --optimize-autoloader
    php app/console cache:clear --env=prod --no-debug
    php app/console assetic:dump --env=prod --no-debug
