pipeline {
 
agent any 


stages { 

stage('Build') { 

steps { 

echo 'Building the app...' 

sh 'echo Build successful!'
            }
        }
        

stage('Test') {

 steps { 

echo 'Running tests...' 
sh 'echo Tests passed!'
            }
        }
        

stage('Deploy') {

 steps { echo 'Deploying the app...' 

sh 'echo App deployed successfully!'
            }
        }
    }
}
