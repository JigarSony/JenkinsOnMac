# JenkinsOnMac

#https://stackoverflow.com/questions/37146063/how-do-i-get-initial-admin-password-for-jenkins-on-mac


https://medium.com/@ved.pandey/setting-up-jenkins-on-mac-osx-50d8fe16df9f

https://www.youtube.com/watch?v=qg9Zt7YPFq8

Please execute the following commands to remove Jenkins completely from Mac. 

1.  /Library/Application\ Support/Jenkins/Uninstall.command

2.  sudo rm -rf /var/root/.jenkins ~/.jenkins

3.  sudo rm -rf /Users/Shared/Jenkins

4.  sudo dscl . -delete /Users/jenkins

5.  sudo dscl . -delete /Groups/jenkins

6.  sudo rm -f /etc/newsyslog.d/jenkins.conf

7.  pkgutil --pkgs | grep 'org\.jenkins-ci\.' | xargs -n 1 sudo pkgutil --
     forget
