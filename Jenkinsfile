pipeline {
    agent any
    
    stages {
        stage ("main"){
            when{
                branch "main"
            }
            steps{
                git branch: 'main', url: 'https://github.com/Esthersurya1223/E-commerce-project-springBoot.git'
            }
            
        }
        stage ("devlop"){
            when{
                branch "build"
            }
            steps{
                sh 'mvn clean package'
            }
            
        }
    }
}
