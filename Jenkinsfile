pipeline {
    agent any

    stages {

        stage('Check Python') {
            steps {
                bat '"C:\\Users\\DELL\\AppData\\Local\\Python\\bin\\python.exe" --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\DELL\\AppData\\Local\\Python\\bin\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\DELL\\AppData\\Local\\Python\\bin\\python.exe" -m pytest'
            }
        }

        stage('Build Success') {
            steps {
                echo 'Build Completed Successfully!'
            }
        }
    }
}
