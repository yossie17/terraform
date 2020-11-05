pipeline {
    agent {
        docker { image 'yossie17/terratorm:v1'}
    }
    stages {
        stage('Test') {
            steps {
                sh 'hostname'
                sh 'terraform -v'
                sh 'ls -la'
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