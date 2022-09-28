pipeline{
    agent any
    stages{
            stage('test') {
                steps {
                    sh 'echo hello,This is for test'
                }
            }
          stage('clone')  {
            steps {
                git url: 'https://github.com/tejaswiqt/spring-petclinic.git',
                    branch: 'main'
            }
          }
            stage('build'){
                steps {
                    sh 'mvn package'

                }
            }
          }
            
        }