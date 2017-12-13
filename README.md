Terraform
=========

Installs terraform on mac os

Requirements
------------

None

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    terraform_install_version: "0.11.1"
    
Version which should be installed

    terraform_download_destination: "/tmp/terraform_{{ terraform_install_version }}.zip"
    
Path which will be used to download terraform

    terraform_unarchive_destination: "/tmp/terraform/"
    
Path which will be used to extract downloaded archive

    terraform_execution_path: "/usr/local/bin/terraform"

Path which will be used to move the extracted file and make it executable

    terraform_releases_url: "https://releases.hashicorp.com/terraform/{{ terraform_install_version }}/terraform_{{ terraform_install_version }}_darwin_amd64.zip"
    
Url to download terraform

Dependencies
------------

None

Example Playbook
----------------

    - hosts: 127.0.0.1
      connection: local
      roles:
         - { role: solutiondrive.terraform }

License
-------

MIT / BSD

Author Information
------------------

This role was created by [solutionDrive](http://solutiondrive.de)
