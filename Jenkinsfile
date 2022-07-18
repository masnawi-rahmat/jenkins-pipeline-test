pipeline {
   agent any
   stages {
       stage('write') {
           steps {
               script {
                   def date = new Date()
                   def data = "Hello World\nSecond line\n" + date
                   writeFile(file: 'zorg.txt', text: data)
                   sh "ls -l"
                   sh "cat zorg.txt" 
               }
           }
       }
       stage('read') {
           steps {
               script {
                   //def data = readFile(file: 'zorg.txt')
                   def data = readFile(file: 'sometext.txt')
                   data.split('\n') 
                   println(data)
                   //println(line)
               }
           }
       }
   }
}
