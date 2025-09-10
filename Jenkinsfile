pipeline{
 agent any
    stages{
        stage('Dir'){
            steps{
                echo 'Hello World'
                sh 'ls -al'
                sh 'pwd'
                sh 'rm -rf build-benchmark'
                sh 'git clone https://github.com/aedm/build-benchmark.git'
                sh 'cd build-benchmark/linux'
                //sh './init-install-toolchains.sh'
                //sh 'init-clone-repos.sh'     
                sh 'pwd'
                sh 'ls -al'
            }
        }
    }
    
}



