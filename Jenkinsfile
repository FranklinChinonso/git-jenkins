pipeline{
    agent any

    stages{
        stage('Code checkout'){
            steps{
                echo "Checking out code from git repository"
                checkout scm

            }
        }

        stage('Run python script'){
            steps{
                echo "Running the python script from the git repository"
                sh 'python3 numbers.py'
            }
        }
    }
    post {
        always {
            echo 'Pipeline execution completed'
        }
    }
}
