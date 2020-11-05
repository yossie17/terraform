// pipeline {
//     agent {
//         docker { image 'hashicorp/terraform'}
//     }
//     stages {
//         stage('Test') {
//             steps {
//                 sh 'terraform -v'
//             }
//         }
//     }
// }


pipeline {
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'terraform -v'
                
            }
        }
    }
}