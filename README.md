# nftables
Firewall

           ----------->

TOR                         SERVIDOR/USER

          <-----------

Filter by:
MACADDRESS   ------>     IP    -------> PORT

Allow only MACADDRESS permited in the PRIVATE NETWORK.
Allow only IP permited in the PRIVATE NETWORK.

Allow only TOR IP with PORT.
Allow only User Level Protocols in SERVIDOR/USER.

Deny the rest MACADDRES in the PRIVATE NETWORK.
Deny the rest IP in the PRIVATE NETWORK.
Deny all TOP IP with no specific PORT.

BLOCK/REDIRECT the rest of PROTOCOLS (system, user and protected) not used.

# Environment:
  Using FEDORA as Operation System.  Minimum installation.
  Uninstall firewalld unbound iptables.
  Install nftables.

# By default:
        All is blocked, macadress IP Protocol.
# In specific:
        Try to block or deny  specific macadress IP Protocol.

# Management:
  Allow only SSH access to specific IP.
  Deny the rest IP in the PRIVATE NETWORK.

# Proxy:
  Allow only SQUID access to specific IP.
  Deny the rest IP in the PRIVATE NETWORK.

# DNS:
  Blocked in the PRIVATE NETWORK.
  Only access via LOCALHOST from SQUID.


