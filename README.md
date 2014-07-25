#LiveVoting

##How to install?

    $ git clone https://github.com/netgen/LiveVoting.git LiveVoting/
    $ cd LiveVoting
    $ mkdir src/
    $ cd src/
    $ mkdir Netgen/
    $ cd NetGen/
    $ git clone https://github.com/netgen/LiveVoting.git LiveVotingBundle/
    $ cd LiveVotingBundle/
    # installing assets
    $ php app/console assets:install --symlink
    # move to production mode
    $ composer install --no-dev --optimize-autoloader
    $ php app/console cache:clear --env=prod --no-debug
    $ php app/console assetic:dump --env=prod --no-debug
