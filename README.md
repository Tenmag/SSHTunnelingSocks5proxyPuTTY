# SSH tunneling Socks5 proxy
### for Firefox with [PuTTY] or [KiTTY]

if: SSH port 22 on server, local proxy port 8080

`plink.exe -v -ssh -x -a -T -C -N -P 22 -D 8080 user@exampleserver.com`  
or  
`klink.exe -v -ssh -x -a -T -C -N -P 22 -D 8080 user@exampleserver.com`

`Store key in cache? (y/n) y`

Firefox <about:config>  
`network.proxy.socks_remote_dns;true`

Set Firefox network connection settings to manual proxy configuration, Socks v5, Socks host 127.0.0.1 port 8080 (check Proxy DNS when using Socks v5).


[PuTTY]: https://the.earth.li/~sgtatham/putty/latest/w32/plink.exe
[KiTTY]: https://www.9bis.net/kitty/?file=klink.exe

