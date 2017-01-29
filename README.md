mlundberg.letsencrypt
=========

Install nginx and letsencrypt for simple hosting of static resources.

Requirements
------------

No host requirements. A dns record must be setup for the target.

Role Variables
--------------

`letsencrypt_domain_name`: The domain name to be used. There must be a working dns pointer for this name for the letsencrypt certificate to be created.

`letsencrypt_email`: Your email address. Required for creation of letsencrypt certificate.

`letsencrypt_extra_location_blocks`: Extra location block config for nginx.

Dependencies
------------

No extrenal dependencies.

Example Playbook
----------------

Example how to use the role within a playbook:

    - hosts: servers
      roles:
         - { role: mattiaslundberg.letsencrypt, letsencrypt_domain_name: "mydomain.com", letsencrypt_email: "me@mydomain.com" }

License
-------

MIT

Author Information
------------------

[Mattias Lundberg](https://mlundberg.se)
