# installation
java and jenkins


#JAVA INSTALLATION IN UBUNTU 

#$ sudo apt update
#$ sudo apt-get install openjdk-8-jdk -y


#JENKINS INSTALLATION

#$ 1. go to jenkins.in site
   2. click on downloads
   3. select your o/s , here i am selected ubuntu
   4. wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add
   5. Then add the following entry in your /etc/apt/sources.list:
      deb https://pkg.jenkins.io/debian binary/
   6. sudo apt-get update
      sudo apt-get install jenkins
   7. start the jenkins server
      systemctl start jenkins
      systemctl status jenkins
      
 #TERRAFROM INSTALLATION
   1.go to terrafrom.io site then got downloads select linux 64 and copy url.
   2.now open putty and connect to server and download terrafrom zip file using below commnad
     $ sudo curl -O https://releases.hashicorp.com/terraform/0.12.18/terraform_0.12.18_linux_amd64.zip
   3. unzip terrafrom zip file.
      $unzip terrafromzipfile
      now you will get terraform executable file, move this file into /etc/loacal/bin/
   4. check terrafrom installed properly or not
     $terraform 
     $terraform -v
