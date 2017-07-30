# Ansible Role: Nginx

[![Build Status](https://travis-ci.org/labpositiva/ansible-role-nginx.svg)](https://travis-ci.org/labpositiva/ansible-role-nginx)
[![GitHub issues](https://img.shields.io/github/issues/labpositiva/ansible-role-nginx.svg)](https://github.com/labpositiva/ansible-role-nginx/issues)
[![GitHub license](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square)](LICENSE)


Installs and configures [nginx][link-nginx] on a host.

## Requirements

 - Linux
   - none
 - OSX
   - [Homebrew][link-brew] must be installed.


## Role Variables

The default role variables in `defaults/main.yml` are:

    ---
    # defaults file for nginx
    nginx_keepalive_timeout: "65"
    nginx_keepalive_requests: "1000"

    nginx_client_max_body_size: "64m"
    nginx_client_body_timeout: "3m"
    nginx_client_header_timeout: "3m"

    nginx_server_names_hash_bucket_size: "64"


## Dependencies

none

## Example Playbook

See the [examples](./examples/) directory.

To run this playbook with default settings, create a basic playbook like this:

    - hosts: servers
      roles:
         - nginx

To install a specific version:

    - hosts: servers
      roles:
         - { role: labpositiva.nginx }


## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

Made with :heart: ️:coffee:️ and :pizza: by [labpositiva][link-company].

- [All Contributors][link-contributors]

[link-nginx]: https://nginx.org/
[link-brew]: http://brew.sh/

[link-contributors]: AUTHORS
[link-company]: https://github.com/labpositiva
