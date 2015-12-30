# synology-gitlab
Updated an improved Original Synology Package from https://www.synology.com/de-de/dsm/app_packages/Docker-GitLab

Packages used:  
https://hub.docker.com/r/sameersbn/gitlab/  
https://hub.docker.com/r/sameersbn/redis/  

NOTES: 
- When cloning please be shure to turn off the git autocrlf, otherwise shell installation scripts may not work.
You can use this command: git config --global core.autocrlf false

#2015-12-31
Improvements
- Gitlab Update to 8.3.2 - sameersbn/gitlab:8.3.2 (254.3MB)  
- Added English UI
- renamed package folder spk/ to bin/
- install/updated/uninstall procces rewrite
- Feature: Uninstall and Keep Gitlab Data
- Feature: Use individual database user and password. 
- Feature: Install on existing gitlab database and files
- Note: On Update you may need to specify the Databse User "gitlab" once



#2015-12-14
Improvements
- Updated Redis to latest
- Gitlab Update to 8.2.3
- Increased UNICORN_TIMEOUT to 180s

The following docker images will be downloaded during the installation. This will take some time so please be ptaient.
sameersbn/gitlab:8.2.3 (249.7MB)  
sameersbn/redis:latest (66MB)
