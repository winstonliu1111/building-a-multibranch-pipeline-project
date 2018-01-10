pipeline {
    agent {
        docker {
            image 'kraney/k8s-nsvc-deploy'
        } 
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello Ixia!"'
                sh 'which kops'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Hello Test"'
                sh 'which kubectl'
                sh 'which terraform'
            }
        }
    }
}
