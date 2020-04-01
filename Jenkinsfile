pipeline {
   agent any
   stages {
      stage('Hello') {
         steps {
           timeout(time: 15, unit: "MINUTES") {
             input message: 'Proceed?', ok: 'Yes'
            }
            echo 'Hello World'
         }
      }
   }
}
