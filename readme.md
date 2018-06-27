# proxyConnector

## HowTo:

If you want to use the TOR Network:

1.  Verify that you have TOR installed in your system or find a TOR Proxy
2.  Write the IP and the PORT of the proxy into the ini file in the [general] section
3.  If you want to control TOR proxy to change identity you need to configure both
    the TOR proxy and the ini file.
    3.1 Configure the TOR Proxy:
    3.1.1: Go to the configuration file of the proxy and enable the control port.
    The configuration file should be placed here: /etc/tor/torrc
    3.1.2: The password need to be setted in the HashedControlPassword
    3.1.3: Set the password: tor --hash-password YOUR_STRONG_PASSWORD

    3.2 The ini file:
    In the tor section write the PORT of the control port you had enable before
    and the password you used to run tor --hash-password YOUR_STRONG_PASSWORD

Thanks.
