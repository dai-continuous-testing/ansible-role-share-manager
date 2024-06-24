Experitest - Share Manager ansible role
=========

This role will install \ uninstall share manager for linux os hosts

Requirements
------------

* Supports linux os hosts only.

Role Variables
--------------

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| state | should the application be present or absent | present, absent | present | no |
| app_version | application version to install | string | 21.5.37 | no |
| server_port | port number for the server | number | 443 | no |
| extra_application_properties | additional props to be override in application.properties file | dict | {} | no |
| installation_root_folder | the root folder in which the application will be installed under mdmserver-{version} folder | string | for linux: /opt/Experitest | no |
| java_version | java jre version to install | string | 8u292-b10 | no |
| custom_download_url | custom url to download the installation from (zip format) | string |  | no |
| custom_download_username | username to download from custom url on windows | string |  | no |
| custom_download_password | password to download from custom url on windows | string |  | no |
| start_after_install | should application start after installation is completed | boolean | True | no |
| clear_temp_folder | remove temp folder after installation | boolean | False | no |
| clear_before_install | removing old installation before installing new version | boolean | False | no |


