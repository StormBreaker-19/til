## On Lightsail

Lightsail adds some junk to the `/home/dokku/.ssh/authorized_keys` file

1. Clear it out

2. Copy your public key somewhere locally

3. Start again with `dokku ssh-keys:add admin /path/to/local/id_rsa.pub`

4. Test it worked with `dokku ssh-keys:list` 
