node{
    def mavenhome = tool name: "maven3.8.2"
    stage('checkoutcode'){
  	git branch: 'development', credentialsId: '8b42bd04-0b4b-4b6b-ac8c-de3d920321fa', url: 'https://github.com/cap-ecom-proj1/maven-web-application.git'
    }
  	stage('build'){
  	sh "${mavenhome}/bin/mvn clean package"
  	}
    /*
  	stage('executesonarqube'){
  	sh "${mavenhome}/bin/mvn clean sonar:sonar"
  	}
  	stage('uploadtonexus'){
  	sh "${mavenhome}/bin/mvn clean deploy"
  	}
    stage('deploytotomcat'){
  	sshagent(['4ed6d9c6-a86d-4b0e-b7fe-82a00547b31f']) {
    sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@3.6.91.154:/opt/apache-tomcat-9.0.53/webapps"
    }
  	}*/
  }
  
