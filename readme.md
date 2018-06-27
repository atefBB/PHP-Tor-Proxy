# Tor proxy connector

## HowTo:

If you want to use the TOR Network:

- Verify that you have TOR installed in your system or find a TOR Proxy
- Write the IP and the PORT of the proxy into the ini file in the [general] section
- If you want to control TOR proxy to change identity you need to configure both
  the TOR proxy and the ini file.

  - Configure the TOR Proxy:

    - Go to the configuration file of the proxy and enable the control port.
      The configuration file should be placed here: /etc/tor/torrc
    - The password need to be setted in the HashedControlPassword
    - Set the password: tor --hash-password YOUR_STRONG_PASSWORD

  - The ini file:
    In the tor section write the PORT of the control port you had enable before
    and the password you used to run tor --hash-password YOUR_STRONG_PASSWORD

Thanks.
