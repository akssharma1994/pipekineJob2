pipeline{
    agent any
    parameters{
        string (name: 'num1', defaultValue: '8', description: '')
        string (name: 'num2', defaultValue: '9', description: '')

    }
    stages{
        stage("Adding a script file"){
            steps{
                readTrusted 'addition.sh'
                sh "chmod +x -R ${env.WORKSPACE}"
                sh ("./addition.sh")
            }
        }   
    }
}