pipeline {
  agent any

    tools {
        nodejs "node"}

    stages {

        stage('Cypress Parallel Test Suite') {
            parallel {
                stage('Slave 1') {
                    agent {
                        label "Agent3_1"
                    }
                    steps {
                        git url: 'https://github.com/jvargas30161/pipline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run cypress run --record --key 7f3ad08e-6c6e-442f-bcbd-cb3269ac5a9c  --parallel'
                    
                    }
                }

        stage('Slave 2') {
                    agent {
                        label "Agent3_2"
                    }
                    steps {
                        git url: 'https://github.com/jvargas30161/pipline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run --record --key 0019ce37-3ac6-44c2-bc8e-1c081c466a39  --parallel'
                    
                    }
                }

        stage('Slave 3') {
                    agent {
                        label "Agent3_3"
                    }
                    steps {
                        git url: 'https://github.com/jvargas30161/pipline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run --record --key 0019ce37-3ac6-44c2-bc8e-1c081c466a39  --parallel'
                    
                    }
                }

        stage('Slave 4') {
                    agent {
                        label "Agent3_4"
                    }
                    steps {
                        git url: 'https://github.com/jvargas30161/pipline.git'
                        bat 'npm install'
                        bat 'npm update'                       
                        bat 'npx cypress run --record --key 0019ce37-3ac6-44c2-bc8e-1c081c466a39  --parallel'
                    
                    }
                }

        stage('Slave 5') {
                    agent {
                        label "Agent3_5"
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