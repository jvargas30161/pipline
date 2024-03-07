pipeline {
    agent any

    tools {nodejs "node"}

    stages {

        stage('Cypress Parallel Test Suite') {
            parallel {
                stage('Slave 1') {
                    agent {
                        label "Agent2_1"
                    }
                    steps {
                        git url: 'https://github.com/jvargas30161/pipline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run --record --key 0019ce37-3ac6-44c2-bc8e-1c081c466a39  --parallel'
                    
                    }
                }

                
                  
            }

             
        }

    }
            
}