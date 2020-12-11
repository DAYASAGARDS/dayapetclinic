# dayapetclinic

Github  
From <https://github.com/DAYASAGARDS/Lab2.1> 

Install Github
 100  git --version
  101  sudo apt-get install get
  102  sudo apt-get install git
  103  git congig --global user.email "vickey.daya@gmail.com"
  104  git config --global user.email "vickey.daya@gmail.com"
  105  git config --global user.username  "dayasagards"




Add commit

115  git init
  116  git add .
  117  git status
  118  git commit . -m "This folder includes all demo files"
  119  git remote add origin https://github.com/DAYASAGARDS/Lab2.1.git
  120  git push -u origin main
  121  git push -u origin master


  123  git pull
  124  git status


Jenkins
From <https://github.com/amitvashisttech/devops301-mindtree-17Oct2020/tree/main/02-Jenkins> 
  apt-get install default-jdk -y
  java -version
  wget https://get.jenkins.io/war-stable/2.249.2/jenkins.war
  mv jenkins.war /root/
Setup Jenkins to run on custom port : 9090
nohup  java -jar /root/jenkins.war --httpPort=9090 > output.txt &
Now you can access the Jenkins via Web Brower, Please go ahead & Complete the Setup process
Get the initial Credentials
 cat /root/.jenkins/secrets/initialAdminPassword
Git Pull / Clone my repo:
sudo su - 
git clone https://github.com/amitvashisttech/devops301-mindtree-17Oct2020.git
cd devops301-mindtree-17Oct2020/02-Jenkins/petclinic-code 
If we need to change the port of jenkins.
115  java -jar jenkins.war --httpPort=8123
service jenkins restart
Install Maven Package Builder
apt-get install maven -y 
mvn --version
Let's Build our Petclinic Code with Maven
mvn clean
mvn compile
mvn test
mvn package


ORRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRRR


From <https://github.com/DAYASAGARDS/Lab2.1>

wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
  134  sudo vi /etc/apt/sources.list
  135  sudo apt-get update
  136  sudo apt-get install jenkins
  151  cd var/lib/jenkins/secrets/initialAdminPassword
 155  cd lib/jenkins/secrets/
  160  npm init --yes



 tomcat

 674  mkdir petclinic
  675  cd petclinic/
  677  git clone https://github.com/amitvashisttech/devops301-mindtree-17Oct2020.git
  679  cd devops301-mindtree-17Oct2020/
  682  apt-get install maven -y
  683  sudo apt-get install maven -y
  684  mvn --version
  685  mvn clean
  687  cd 02-Jenkins/
  689  cd petclinic-code/
  691  mvn compile
  692  mvn test
  693  mvn package
  694  sudo wget https://archive.apache.org/dist/tomcat/tomcat-8/v8.5.56/bin/apache-tomcat-8.5.56.zip
  696  apt-get install unzip -y
  697  sudo apt-get install unzip -y
  698  unzip apache-tomcat-8.5.56.zip
  700  cp -rf apache-tomcat-8.5.56 /opt/tomcat
  701  sudo cp -rf apache-tomcat-8.5.56 /opt/tomcat
  706  sudo cp -rf 03-Tomcat/tomcat-users.xml   /opt/tomcat/conf/tomcat-users.xml
  707  cat 03-Tomcat/tomcat-users.xml
  708  sudo cp -rf 03-Tomcat/context.xml  /opt/tomcat/webapps/manager/META-INF/context.xml
  709  sudo cd /opt/tomcat/
  710  cd /opt/tomcat/bin
  715  sudo chmod +x catalina.sh 
  716  ./bin/catalina.sh start
  718  ./catalina.sh start
  719  sudo ./catalina.sh start
  720  ps -ef | grep -i tomcat
  721  netstat -tulnp | grep -i 8080
  724  cd /home/dayasagarsalian/Desktop/dayapetclinic/petclinic-code/
  725  git init
  726  git add .
  727  git status
  728  git commit . -m "First commit for my code"
  729  git remote add origin https://github.com/DAYASAGARDS/dayapetclinic.git
  730  git push -u origin main
  731  git remote add origin https://github.com/DAYASAGARDS/dayapetclinic.git
  732  git push -u origin master
  733  git remote add origin https://github.com/DAYASAGARDS/dayapetclinic.git
  734  git push -u origin main
  735  git push -u origin master
  736  ps -ef | grep -i tomcat
  737  netstat -tulnp | grep -i 8080
  738  netstat -tulnp
  739  netstat -tulnp | grep -i 8080
  740  ps -ef | grep -i tomcat





Docker hub

  97  docker login --username=dayasagards --password=Sherilyn@123
 104  docker push dayasagards/demomysql:5.7
