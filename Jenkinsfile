pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                //sh "sudo npm install"
                //sh "cd jenkins-react-app && sudo npm run build"
                sh "ls -a"
                sh "pwd"
            }
        }
        stage("Deploy") {
            steps {
                sh "sudo cp -r ${WORKSPACE}/build/ /var/www/jenkins-react-app/build/"
            }
        }
    }
}
