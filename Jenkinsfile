pipeline {
    agent any

    environment {
            currentEnvName = envName(env.BRANCH_NAME)
            installNeeded = requireInstall(env.BRANCH_NAME)

    }
    
    stages {
        stage('Create Environment') {
            steps {
                echo "Nombre Ambiente: ${currentEnvName}"

            }
        }

        stage('Build') {
            steps {
                echo "building... ${env.BUILD_ID} on ${env.JENKINS_URL} ${env.JOB_NAME}"
            }
        }
        stage('Test') {
            steps {
                echo "testing... ${env.BUILD_ID} on ${env.JENKINS_URL} ${env.JOB_NAME}"
            }
        }

    }
    

}
