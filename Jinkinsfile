node {
 
 stage('Git CheckOut') {
    git branch: 'main', url: 'https://github.com/amitvashisttech/devops301-mindtree-17Oct2020.git'
 }
 
 def project_path="02-Jenkins/petclinic-code"
 
 dir(project_path) {
 
 stage('Maven Clean') {
    sh 'mvn clean'
 }
 
  stage('Maven Compile') {
    sh 'mvn compile'
 }
 
 stage('Maven Testing') {
    sh 'mvn test'
 }
 
 stage('Maven Package') {
    sh 'mvn package'
 }
 
 stage('Archive Artifacts') {
    archive 'target/*.war'
 }
}
 
}
