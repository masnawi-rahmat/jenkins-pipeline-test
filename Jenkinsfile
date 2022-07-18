pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello world 00'
            }
        }
    }
        stage('read file'){
            steps {
                script {
                pritln("test print line")
                    def readtext = readFile(file: 'sometext.txt')
                        readtext.split('\n').each{ line ->
                        println(line)
            }            
        }    
              
     }
}
