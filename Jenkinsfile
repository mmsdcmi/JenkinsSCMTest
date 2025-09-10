pipeline{
 agent any
    stages{
        stage('Dir'){
            steps{
            sh script:'''
          #!/bin/bash
          rm -rf build-benchmark
          git clone https://github.com/aedm/build-benchmark.git
          
          
        '''
           dir('build-benchmark/linux') {
                 sh './init-install-toolchains.sh' 
                 sh './init-clone-repos.sh'
                 sh './bench-rust.sh'
              }               
                 
               
            }
        }
    }
    
}



