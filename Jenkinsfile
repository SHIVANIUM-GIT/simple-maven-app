pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/SHIVANIUM-GIT/simple-java-maven-app.git'
            }
        }
        // stage('Build') {
        //     steps {
        //         sh '''
        //         cd simple-java-maven-app
        //         mkdir folder
        //         mvn clean package
        //         '''
        //     }
        // }
        // stage('Build Docker Image') {
        //     steps {
        //         script {
        //             sh '''
        //             cd simple-java-maven-app
        //             docker build -t shivanium/javaweb:${DOCKER_TAG} .
        //             '''
        //         }
        //     }
        // }
        // stage('Push Docker Image on Docker Hub') {
        //     steps {
        //         script {
        //             sh "docker push shivanium/javaweb:${DOCKER_TAG}"
        //         }
        //     }
        // }
        // stage('Deploy') {
        //     steps {
        //         sh '''
        //         cd simple-java-maven-app
        //         java -jar target/*.jar
        //         '''
        //     }
        // }
    }
}
