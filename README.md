proxy-checker
=============
Scrapes SOCKS proxies of the Internet, checks whether they are working or not, and where they are located. It can also check user provided proxies

Usage
=============
usage: ./proxyChecker.py [options]
            Options:
            
            -r, --regular                     scrapes SOCKS proxies off the internet, checks
                                              whether it's working and retrieves its location
            -s [ip:port], --single=[ip:port]  tests whether user given proxy is working, and
                                              retrieves its location
            -L [listfile], --list=listfile    tests the proxies from the given list file, and
                                              retrieves their locations (proxies in format IP:Port)
            -l [logfile], --log=logfile       logs all the output into a log file (info will not be
                                              logged if you exit the program before it stops running
            -p [type], --proxyType=type       proxyType is required, when user provided proxy or
                                              list of proxies are tested (if proxies in the list are
                                              of different format, use option -U)
            -U, --unknownType                 must be enabled if not proxyType provided for user
                                              provide proxies (this might take quite a while)
            -n, --noLocation                  only tests the proxy(ies), but does not retrieve location
            -N, --noTesting                   only retrieves the location(s) of the proxy(ies),
                                              but does not test
             
            -h                                shows this help menu
