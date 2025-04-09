# LSM - Laravel Server Manager
Managing a server properly requires a great deal of specialized knowledge.  Additionally it can be easy to make a mistake and leave a back door open on a server.  The goal here is to allow a single PC to manage multiple servers, quickly installing the necessary software packages, configuring it and locking it down against intrusion.  This is not an easy task.  Even when it is, it's easy to make a mistake.  LSM is here to help.

# Definitions
PC - the computer which manages the Laravel-hosting servers.  Usually this is your workstation.
Server - the server, usually a droplet, which hosts a laravel website.  There can be any number of servers.  Eventually I will be supporting other server types.

# Central "PC" manager
One central PC (usually your workstation) manages your servers by helping you:
- Upload LSM updates to the remote Servers
- Pull configuration changes from each remote server to the PC as a backup
- Manage many remote servers

# Managing servers
The Laravel hosting server is usually a Droplet, but I hope to allow other server types in the future.
This project allows the user to do the following, starting from a bare-bones droplet:
- Install necessary packages and software, including: Letsencrypt, NTP server, nginx, postfix, PHP 8.3+, nmap, etc.
- Configure necessary packages, including firewall.
- Evaluate any server for security holes and fix them automatically.
- Manage deployments

# Managing websites
This project supports website management including:
- Multiple websites on a single server with different ports.
- Auto-generation of nginx configuration files with Letsencrypt certificates.
- Backup restoration of spatie-backup files with rollback support.
- Copying of an existing website with rollback support.
- Github update of an existing website with rollback support.

# LSM is designed to support servers on-premises 
- Where GitHub Continuous Deployment would be unsuitable.
- More secure not giving GitHub access to your server.
- Your server can remain on-premises.
- Your server can be hosted behind a firewall with no direct public access.

  
