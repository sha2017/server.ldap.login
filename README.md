LDAP PAM Client
=========

Role that deploys PAM connection to an LDAP server using LDAP bind. 

Requirements
------------
Debian

Role Variables
--------------

domain_base: LDAP Search Domain
uri: Uri string of LDAP server.


Dependencies
------------
none

Example Playbook
----------------
The following vars are used to link PAM to an LDAP server. 
  vars:
    openldap_:
      domain_base: "dc=domain,dc=local"
      uri: "ldap://ldap1.domain.local/"
      binduser: "cn=admin,dc=domain,dc=local"
      bindpw: "12345678"


License
-------

GPL

Author Information
------------------
Peter Tambach
Matthew Frost

