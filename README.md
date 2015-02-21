# Casper - Revised

This repo is a revision of the default theme [Ghost](http://github.com/tryghost/ghost/).

## Pushing Update to AWS

To push to the AWS site
- First push update to git repo
- `ssh -i ghost-blog.pem XXX.amazonaws.com`  # XXX = Your Amazon Public IP

Once ssh'd into server 
- `cd /var/www/ghost/content/themes/blog-theme`
- `git pull origin master` # update from gitreop
- `pm2 restart ghost` # restart ghost


## Copyright & License

Copyright (c) 2013-2015 Ghost Foundation - Released under the MIT License.