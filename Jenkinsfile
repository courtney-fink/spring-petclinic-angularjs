pipeline {
    agent any

 

    stages {
        stage('Hello') {
            steps {
                sh '''#!/bin/bash
                
                    git clone https://github.com/spring-petclinic/spring-petclinic-angularjs.git
                    cd spring-petclinic-angularjs
                    ./mvnw clean install
                    cd spring-petclinic-server
                    ../mvnw spring-boot:run
                '''
            }
        }
    }
}
