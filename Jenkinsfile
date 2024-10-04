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
                   bat '"C:\\Program Files\\Microsoft Visual Studio\\2022\\Professional\\MSBuild\\Current\\Bin\\MSBuild.exe" /t:Rebuild /p:Configuration=Debug HelloWorld.sln'

            }
        }
  }
}
