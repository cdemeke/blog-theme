# Casper - Revised

This repo is a revision of the default theme [Ghost](http://github.com/tryghost/ghost/).
###[Demo](http://chrisdemeke.com/)

## Pushing Update to AWS

If this your first time here is a [good resource to set up your Ghost and AWS website and add a custome theme] (http://dannydelott.com/installing-ghost-blog-on-amazon-web-services-with-namecheap-domain-and-custom-theme/)


To push to the AWS site
- First push update to git repo
- `ssh -i ghost-blog.pem XXX.amazonaws.com`  # XXX = Your Amazon Public IP

Once ssh'd into server 
- `cd /var/www/ghost/content/themes/blog-theme`
- `git pull origin master` # update from gitreop
- `pm2 restart ghost` # restart ghost


## Copyright & License

Copyright (c) 2013-2015 Ghost Foundation - Released under the MIT License.