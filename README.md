# Reset-Jenkins-password

jenkins password reset steps 

# steps 
here are the steps you need to follow :
# step 1 : choose your distribution 
Mac os : /Users/your_mac_username_folder/ .jenkins
linux : /var/lib/jenkins
# step 2 : 
find the config.xml file and edit the **<useSecurity>true</useSecurity>** to **<useSecurity>false</useSecurity>** & save the file 
# step 3 : 
restart your jenkins using brew services stop jenkins-lts for macos || systemctl jenkins restart for ubuntu or linux
# step 4 :
now you will see jenkins will disabled the login and will open automatically 
# step 5 : 
manage jenkins >> system security >> choose **jenkins own user database** on the configure global security page >> apply >> save 
# step 6 :
now go to people >> check userid (for which password will be reset) >> scroll down choose password and click apply & save 

# step 7 : lastly please change the config.xml file again by putting **<useSecurity>true</useSecurity>** and restart your jenkins .
