pipeline {
    agent {
        docker { image 'ubuntu'}
    }
    stages {
        stage('Test') {
            steps {
                sh 'hostname'
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
                
//             }
//         }
//     }
// }