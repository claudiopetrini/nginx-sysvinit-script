# nginx SysVinit script
[Linux Standard Base (LSB)](http://www.linuxfoundation.org/collaborate/workgroups/lsb) compliant [SysVinit]
(http://freecode.com/projects/sysvinit) script for [nginx](http://nginx.org/).

## Install
```shell
wget -O /etc/init.d/nginx https://raw.githubusercontent.com/Fleshgrinder/nginx-sysvinit-script/master/nginx
chmod 0755 /etc/init.d/nginx
chown root:root /etc/init.d/nginx
update-rc.d nginx defaults
```

You can also clone the repository and just execute the `install.sh` script.

## Usage
You can use it via the `service` command or by directly invoking the shell script in `/etc/init.d`; what you like best. 
Your shell will have auto-completion for the various keywords that are available, for instance if you type `service 
nginx res` just hit tab for auto-completion.

```shell
service nginx force-reload
service nginx reload
service nginx restart
service nginx start
service nginx status
service nginx stop
```

## Weblinks
* [LSBInitScripts - Debian Wiki](https://wiki.debian.org/LSBInitScripts)

## Nginx PID
The nginx process MUST have pid in /run/nginx.pid


## License
> This is free and unencumbered software released into the public domain.
>
> For more information, please refer to <http://unlicense.org>
