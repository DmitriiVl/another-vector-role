pipeline {
    agent {
      label 'jenkins-agent'      
    }
    stages {
        stage('First') {
            steps {
                sh 'git clone https://github.com/DmitriiVl/another-vector-role.git .'
                sh 'molecule --version'
            }
        }
        stage('Second') {
            steps {
                sh 'molecule test -s centos7'
            }
        }    
    }
}