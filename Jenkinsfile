pipeline {
    agent {
        docker { image 'yossie17/terratorm:v2'}
    }
    stages {
        stage('AWS-Credentials') {
            steps {
                sh 'hostname'
                sh 'mkdir /root/.aws/'
                sh 'envsubst  < credentials.template > /root/.aws/credentials'
            }
        }
        
        stage('Test') {
            steps {
                sh 'hostname'
                sh 'terraform -v'
                sh 'terraform init amazon/terraform'
                sh 'terraform plan amazon/terraform'

            }
        }
    }
}


// pipeline {
//     agent { dockerfile true }
//     stages {
//         stage('Test') {
//             steps {
//                 sh 'terraform -v'
//                 sh 'ls -la'
                
//             }
//         }
//     }
// }