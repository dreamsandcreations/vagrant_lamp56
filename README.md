# vagrant_lamp56

## Aan te passen in puphpet/config.yml

vagrantfile:

    vm:
    
        hostname: local.puphpet                 <- hernoem naar local-PROJECT.puphpet
        network:
            private_network: 192.168.56.101     <- zet naar correct ip
            forwarded_port:
                vflnp_5zttq7xwsgwm:
                    host: '9101'                <- zet naar 91 + laatste 2 cijfers van ip: 
                    
    apache:
        vhosts:
            av_4yzvuotkefrk:
                servername: awesome.dev         <- zet naar gewenst domein
                serveraliases:
                    - www.awesome.dev           <- zet naar gewenst domein
                    
## ssh key voor sequal pro:

puphpet/files/dot/ssh/id_rsa
