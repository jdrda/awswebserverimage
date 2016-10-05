# awswebserverimage
Performance-based installation of Amazon EC2 micro (free tier) with Apache, PHP and GIT
## Background
As I have created many webservers on Amazon Web Services (AWS) installations for my customers, I found how to tune it to maximum performance.
So I created image for the community to help other developer to set up this great service
## Current version 1.0
### Software
* Amazon Linux defaults + following
* Apache HTTPD 2.4 with MOD SSL and MOD PageSpeed
* PHP 7.0 with all necessay extensions included opcache, mbstring, mcrypt, etc.
* GIT versioning system
* Local clients for MySQL 5.6 and Postgresql 9.5
* Midnight Commander
### Configuration
* 1GB Swapfile with swappinness = 0 (use only if RAM is not available)
* Example configuration for website (/etc/httpd/conf.d and /etc/httpd/vhosts)
* PHP with reduced RAM consuption, errors turned on
* Timezone set to /Europe/Prague
### Hardware
* System HDD 8GB
* Data HDD 10GB mounted to /var/www/html (no deletion with instance)

Good luck!
