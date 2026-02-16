# forge-artisan

For usage on Forge-managed servers with website isolation, where sites are running different php versions. Rather than needing to remember or find which sites are running which php versions, this script pulls it automatically from the nginx config.

### Instructions:

Run these commands once as root:

`sudo curl https://raw.githubusercontent.com/inigopascall/forge-artisan/master/artisan -o /usr/local/bin/artisan`
`sudo chmod +x /usr/local/bin/artisan`

Now whenever you run `artisan` as any site user, it'll prepend the correct php version and run e.g. `php8.2 artisan`.
