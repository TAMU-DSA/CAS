# Limited Life Time Fork

This fork of subfission/cas is intended as a temporary stop-gap until our Laravel 12 apps have a suitable
 replacement. After our internal apps have moved away from this package it will be removed without notice.

- Texas A&M University Technology Services

---

# Repository Archival Notice – Feb 2025
As of June 2024, the apereo/phpCAS repository is no longer actively maintained or updated and we have seen no progress on finding new maintainers. As a result, this codebase remains in a stagnant state with end-of-life (EOL) dependencies. To mitigate security risks for new projects, this repository is now scheduled for immediate archival.

We strongly recommend exploring alternative CAS solutions for future development.

- IT

--- 

# CAS
Simple CAS Authentication for Laravel 6-12.x.

This version of CAS, or Central Authentication Service, is designed to integrate with Laravel 6-11 projects that need to implement SSO.  
Older version of Laravel may work, but are untested. This package was built for my necessity but can be easily used for anyone requiring CAS/SAML SSO in Laravel 6+.  This package is different in mindset as the goal in this project is to be as minimal as possible while offering as much flexibility as needed.

This package offers and abstraction of [Apereo CAS](https://www.apereo.org/projects/cas) (phpCAS), a cross platform and open-source *CAS client* and *server* provider.  Be sure to check them out if you intend to implement an SSO service other than AD.

Check out the [wiki](https://github.com/subfission/cas/wiki) for further details.

## ChangeLog

### Release 5.0.0

* Support added for Laravel 11.x
* Added phpCAS log control
* Refactor internal design to support tests
* Add GitHub actions to run tests and linting

### Release 4 and earlier

* Support added for Laravel 10.x
* Dropped support for phpCAS <1.6.0 (dependency vulnerability)
* Support added for Laravel 9.x
* Support added for Laravel 8.x
* Support added for Laravel 7.x
* Updated for Laravel 6.x
* Dropped support for PHP 5.x
* Laravel 5.5 Package Discovery support
* CAS logout method supports redirection service as a secondary argument
* Supports additional CAS versions, including version 1,2,3
* Supports direct phpCAS calls for heavily customized CAS configurations
* Supports logon with custom URL redirects
* Supports logoff with redirect callbacks
* Updated to work with Laravel 5.2 (backwards compatible)
* Uses the latest phpCAS
* Supports verbose logging
* Session handling has been removed from CAS Manager and is moved strictly into the middleware
* You can now leverage the CAS sessions instead of relying on Laravel sessions
* More security fixes
* Cleaner codebase
* Backwards compatible (for the most part)
* More configuration options in the config file available
* Masquerading as a user now supported
* Tested and working with PHP 7.x
