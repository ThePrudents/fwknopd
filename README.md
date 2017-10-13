fwknopd - Advanced port knocking
================================

[![Build Status](https://travis-ci.org/ThePrudents/fwknopd.svg?branch=master)](https://travis-ci.org/ThePrudents/fwknopd)

Ansible role for setting up jump/bastion server with fwknopd.

Usage
-----

Configuration:
```YAML
users:
  sample_user:
    key_base64: "YOUR_GENERATED_KEY"
    hmac_base64: "YOUR_GENERATED_HMCA_KEY"
    fw_access_timeout: 30 # OPTIONAL
```

Simple usage:

```YAML
---
- hosts: all

  roles:
    - {
        role: "theprudents.fwknopd"
        users:
          sample_user:
            key_base64: "YOUR_GENERATED_KEY"
            hmac_base64: "YOUR_GENERATED_HMCA_KEY"
      }
```


Advanced usage:

```YAML
  ### TODO: Place configuration example here
```


Copyright and license
---------------------

Code licensed under the [MIT License](http://opensource.org/licenses/MIT).
