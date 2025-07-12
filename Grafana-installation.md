
## Grafana:
#### https://grafana.com/grafana/download?platform=linux

---
    [root@infra-01 ~]#  dnf install -y https://dl.grafana.com/enterprise/release/grafana-enterprise-12.0.2-1.x86_64.rpm
    Updating Subscription Management repositories.
    Unable to read consumer identity
    
    This system is not registered with an entitlement server. You can use "rhc" or "subscription-manager" to register.
    
    Last metadata expiration check: 0:39:44 ago on Sat 12 Jul 2025 09:06:52 AM +07.
    grafana-enterprise-12.0.2-1.x86_64.rpm                                                                                                   3.6 MB/s | 174 MB     00:48    
    Dependencies resolved.
    =========================================================================================================================================================================
     Package                                        Architecture                       Version                                Repository                                Size
    =========================================================================================================================================================================
    Installing:
     grafana-enterprise                             x86_64                             12.0.2-1                               @commandline                             174 M
    
    Transaction Summary
    =========================================================================================================================================================================
    Install  1 Package
    
    Total size: 174 M
    Installed size: 642 M
    Downloading Packages:
    Running transaction check
    Transaction check succeeded.
    Running transaction test
    Transaction test succeeded.
    Running transaction
      Preparing        :                                                                                                                                                 1/1 
      Installing       : grafana-enterprise-12.0.2-1.x86_64                                                                                                              1/1 
      Running scriptlet: grafana-enterprise-12.0.2-1.x86_64                                                                                                              1/1 
    ### NOT starting on installation, please execute the following statements to configure grafana to start automatically using systemd
     sudo /bin/systemctl daemon-reload
     sudo /bin/systemctl enable grafana-server.service
    ### You can start grafana-server by executing
     sudo /bin/systemctl start grafana-server.service
    
    POSTTRANS: Running script
    
      Verifying        : grafana-enterprise-12.0.2-1.x86_64                                                                                                              1/1 
    Installed products updated.
    
    Installed:
      grafana-enterprise-12.0.2-1.x86_64                                                                                                                                     
    
    Complete!
---
    http://<localhost>:3000
    http://<ip-address>:3000

    #First login use:
    user=admin
    pasword=admin

 ---   

