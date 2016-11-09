sa-swagger-ui
=============

[![Build Status](https://travis-ci.org/softasap/sa-swagger-ui.svg?branch=master)](https://travis-ci.org/softasap/sa-swagger-ui)

Swagger UI is a dependency-free collection of HTML, Javascript, and CSS assets that dynamically generate beautiful documentation and sandbox from a Swagger-compliant API. Because Swagger UI has no dependencies, you can host it in any server environment, or on your local machine

Example of usage (all parameters are optional)

Simple

  roles:
    - {
        role: "sa-swagger-ui"
      }


Advanced:


  roles:
    - {
        role: "sa-swagger-ui",
        option_install_nodejs: true,
        swaggerui_version: 2.1.4,
        install_dir: /var/www/swagger,
        nodejs_version: "4.x"
      }




