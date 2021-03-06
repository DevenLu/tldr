# ssh-keygen

> Generate ssh keys user for authentication, password-less logins, and other things.

- Generate a key interactively:

`ssh-keygen`

- Specify file in which to save the key:

`ssh-keygen -f ~/.ssh/{{filename}}`

- Generate a DSA 2048 bit (default) key:

`ssh-keygen -t dsa`

- Generate an RSA 4096 bit key with your email as a comment:

`ssh-keygen -t rsa -b 4096 -C "{{email}}"`

- Retrieve the key fingerprint from a host (useful for confirming the authenticity of the host when first connecting to it via SSH):

`ssh-keygen -l -F {{remote_host}}`

- Retrieve the fingerprint of a key in MD5 Hex:

`ssh-keygen -l -E md5 -f ~/.ssh/{{filename}}`

- Change the password of a key:

`ssh-keygen -p -f ~/.ssh/{{filename}}`
