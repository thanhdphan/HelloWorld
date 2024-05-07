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
                   bat '"C:\\Program Files (x86)\\Microsoft Visual Studio\\2017\\Community\\MSBuild\\15.0\\Bin\\MSBuild.exe" /t:Rebuild /p:Configuration=Debug HelloWorld.sln'

            }
        }
  }
}