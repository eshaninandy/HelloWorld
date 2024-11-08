pipeline {
    agent any
    stages {
        stage('Run Complex Tests in Parallel') {
            parallel {
                stage('Addition Tests') {
                    steps {
                        sh 'python -m unittest test_addition_loop'
                    }
                }
                stage('Subtraction and Multiplication Tests') {
                    steps {
                        sh 'python -m unittest test_subtraction_multiplication'
                    }
                }
                stage('Square and Sqrt Tests') {
                    steps {
                        sh 'python -m unittest test_square_and_sqrt_loop'
                    }
                }
                stage('Combined Operations') {
                    steps {
                        sh 'python -m unittest test_combined_operations'
                    }
                }
                stage('Complex Operations and Load Test') {
                    steps {
                        sh 'python -m unittest test_complex_operations'
                    }
                }
            }
        }
    }
}
