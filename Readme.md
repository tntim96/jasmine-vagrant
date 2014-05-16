Download [debian80.box](https://downloads.sourceforge.net/project/vagrantboxjessie/debian80.box)
(list from http://www.vagrantbox.es/).

# Install dependency packages
`sudo apt-get update && sudo apt-get install git-core curl build-essential openssl libssl-dev`

# Install NodeJS
`git clone https://github.com/joyent/node.git`
`cd node`
`git checkout v0.10.28`
 
`./configure --openssl-libpath=/usr/lib/ssl`
`make`
`#make test`
`sudo make install`
`node -v`
`npm -v`
`sudo npm install -g grunt-cli`


# Ruby (+ extra will take some time)
`curl -L https://get.rvm.io | bash -s stable --rails`

# Checkout Jasmine (if not using mapped drive)
`git clone`
`cd jasmine`
`bundle`

# Run Tests
`grunt execSpecsInNode`
`bundle exec rake jasmine`

Port 8888 is forwarded, so you can run tests by going to http://localhost:8888/