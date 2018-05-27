# Generating ssh keys

On your *local* machine 
```sh
$ cd /home/username/.ssh/
$ ssh-keygen -t rsa -b 2048
```

choose the file name for your keys to be saved and a passphrase for your private key ( you will be asked for this passphrase everytime you try to login with your private key, you can leave it blank if you are bored to type it every time.)

Check your keys being generated with:
```sh
$ ls -lahrt /home/username/.ssh
```

# Server Side
Now your public key needs to be installed on the server machine.
Contact us and send us your public key (filename.pub), not the private key, keep that one safe and dont lose it.

Contact info: svretina@physics.auth.gr , stzaneti@physics.auth.gr
email subject: deathstar

or come by the IT Department which is located on the 4th floor of the "Glass" building.

# Logging in

If you have both your public and private key saved in the /home/username/.ssh/ you can use
```sh
$ ssh username@hostdomain
```
and log in. If you saved it somewhere else you have to run the -i flag to specify the custom location of the keys:
```sh
$ ssh -i /path/to/your/keys username@hostdomain
```
( so better move them to the /home/username/.ssh directory )

enjoy your stay at the DeathStar!

