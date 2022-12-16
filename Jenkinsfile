pipeline{

agent any
stages('CI CD Pipeline'){
  stage('Code Checkout'){
    steps{
        script{
            git credentialsId: 'e45b78ae-2b32-45d1-a8d7-b789028d9b24', url: 'https://github.com/shrth7/Inventory-Management-System-Spring-Boot.git'
            }
        } 
    }

  stage('Build'){
    steps{
        script{
            sh "mvn clean install -Dmaven.test.skip=true"
        }
    }  
  }
  /*stage('Test'){
    steps{
        script{
            sh "mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent install -Pcoverage-per-test"
        }
    }  
  }*/

}
}
