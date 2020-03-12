stage ("Build") {
    node (){
        echo 'building the artifact'
        sleep 2
            }        
          }    

stage ("QA Test") {
   node () {
    timeout(time: 5, unit: 'MINUTES'){
        echo "QA tests..."
        sleep 2
       }
    } 
  }

stage ("Perf Test") {
   node () {
        input 'execute perf Tests?'
        echo "executing Performance tests"
        sleep 2
    } 
  }

stage ("Deploy") {
   node () {
        timeout(time: 5, unit: 'MINUTES'){
            input 'Deploy on load test environment?'
            echo "deploying to test environment."
         }
        sleep 2
  } 
}
