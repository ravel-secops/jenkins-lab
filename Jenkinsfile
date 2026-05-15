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
                    whoami
                    ls -lah ../
                    echo "Teste 001"
                    cd "../Teste 001"
                    ls -lah
                    cd artefatos
                    ls -lah
                    echo "binário simulado" > build/app.bin
                    sleep 2
                '''
            }
        }
    }
}
