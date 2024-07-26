pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/SHIVANIUM-GIT/simple-java-maven-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'cd simple-java-maven-app'
                sh 'mkdir floder'
                sh 'mvn clean package'
            }
        }
        // stage('Build Docker Image') {
        //     steps {
        //         script {
        //             sh "docker build -t shivanium/javaweb:${tag} ."
        //         }
        //     }
        // }
        // stage('Push Docker Image on Docker Hub') {
        //     steps {
        //         script {
        //             def tag = 'latest'
        //             sh "docker push shivanium/javaweb:${tag}"
        //         }
        //     }
        // }
        stage('Deploy') {
            steps {
                sh 'java -jar target/*.jar'
            }
        }
    }
}