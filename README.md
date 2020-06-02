# hamachi-minecraft-server




# Linux setup:

    http://download1.rpmfusion.org/nonfree/fedora/
    https://coderwall.com/p/rkz4_w/installing-hamachi-logmein-in-fedora-20
    https://wiki.ubuntuusers.de/LogMeIn_Hamachi/
 
 
 
----------------
    
# Hamachi for fedora:

After setting up your account in the website, download the source code from https://secure.logmein.com/products/hamachi/download.aspx. Then install the rpm with:

    $ rpm -ivh logmein-*******.rpm 

Login and start:

    $ sudo hamachi login
    $ sudo /etc/init.d/logmein-hamachi start

Add your email in the configuration file:

    $ sudo  subl /var/lib/logmein-hamachi/h2-engine-override.cfg
    $ sudo /etc/init.d/logmein-hamachi restart

Add the network id:

    $ hamachi join 242-045-601
    $ sudo hamachi list

You can also use a GUI: http://software.opensuse.org/download.html?project=home:ztefn&package=haguichi.

----------------




# Gateway Konfifuration:
    
    hamachi gw-config <network id>
                    [dhcp|static [net <start ip> <end ip> <netmask> <default gateway>]
                                 [domain <dns domain>]
                                 [dns <dns ip 1> [<dns ip 2>]]]
                    [del <remote subnet CIDR> ...]
                    [add <remote subnet CIDR> ...]
                   
.
Problme und Vorrausetzungen:

    https://community.logmein.com/t5/LogMeIn-Hamachi-Discussions/How-to-install-a-Hamachi-gateway-PC/td-p/32481
    
    







# Windows setup:

    https://hamachi.de.softonic.com/
    

