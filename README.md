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


##Generating joind.in access token

- Create api-key and secret on `http://joind.in/user/main` -> API Keys item on right side
 with callback on some random url
- Send request `http://joind.in/user/oauth_allow?api_key=[api-key]&callback=[callcal_url]`
- Obtain access token from query param in callback url
