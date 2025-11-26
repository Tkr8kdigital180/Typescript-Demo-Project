pipeline{
    agent{
        label "any"
    }
    stages{
        stage("Install"){
            steps{
                sh "npm install"
            }
        }  
        stage("Build"){
            steps{
                sh "npm run build"
            }
        }  
        stage("Test"){
            steps{
                sh "npm test"
            }
        }  
        stage("Audit"){
            steps{
                sh "npm audit"
                sh "npm audit fix"
                sh "npm outdated"
                sh "npm update"
            }    
        }     
            
        }

        post{
                success{
                    cleanWs()
                }
                failure{
                    echo "Ein Fehler ist aufgetreten"
                }
            }


    }