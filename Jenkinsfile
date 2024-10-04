pipeline {

    agent {
        node {
            label 'master'
        }
    }

	stages {
        stage('Checkout') {
            steps {
                    git 'https://github.com/thanhdphan/HelloWorld.git'

            }
        }

        stage('Build') {

            steps {
                   bat 'MSBuild.exe /t:Rebuild /p:Configuration=Debug HelloWorld.sln'

            }
        }
  }
}
