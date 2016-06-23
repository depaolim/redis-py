# Just a personal memento...

sudo apt-get purge vagrant*
sudo apt-get purge virtualbox*

sudo apt-get install virtualbox  # 4.3.36
sudo apt-get install vagrant  # 1.4.3

# il seguente passo non serve su vagrant>=1.5
vagrant box add hashicorp/precise64 http://atlas.hashicorp.com/hashicorp/boxes/precise64

# per liberare le porte standard di redis
service redis-server stop

cd vagrant

# avvio della macchina virtuale
vagrant up

# stop della macchina virtuale
vagrant halt

# eventuale distruzione della macchina virtuale
# vagrant destroy
