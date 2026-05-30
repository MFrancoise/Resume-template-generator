pipeline {
    agent any
    
    stages {
        stage('Display Build Info') {
            steps {
                sh """
                echo ${env.BUILD_NUMBER}
                echo ${env.JENKINS_URL}
                sleep 5
                """
            }
        }
        stage('Display SCM Info') {
            steps {
                sh """
                echo ${env.CHANGE_AUTHOR}
                echo ${env.CHANGE_URL}
                echo ${env.CHANGE_AUTHOR_EMAIL}
                echo ${env.CHANGE_AUTHOR_DISPLAY_NAME}
                sleep 5
                """
            }
        }
    }
}