### Install Plugin
`$ curl -o /usr/share/munin/plugins/ipv6_ https://raw.githubusercontent.com/MorbZ/munin-ipv6/master/ipv6_`  
`$ chmod +x /usr/share/munin/plugins/ipv6_`  

### Setup Graphs
Total throughput:  
`$ ln -s /usr/share/munin/plugins/ipv6_ /etc/munin/plugins/ipv6_total`

Percentages:  
`$ ln -s /usr/share/munin/plugins/ipv6_ /etc/munin/plugins/ipv6_percent`

Don't forget to restart Munin after changing plugins:  
`$ service munin-node restart`
