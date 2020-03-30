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
        input message: 'Should I fail? Yeah, I should.', id:'Icecream'
       }
    } 
  }

stage ("Perf Test") {
   node () {
        echo "executing Performance tests"
        sleep 2
    } 
  }

stage ("Deploy") {
   node () {
        timeout(time: 5, unit: 'MINUTES'){
            echo "deploying to test environment."
         }
        sleep 2
  } 
}
