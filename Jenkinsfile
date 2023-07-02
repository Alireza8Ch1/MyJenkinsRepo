pipeline{
        agent any
          stages{
                stage("one"){
                steps{
                  echo "first stage done!!"
                 }
                }
                stage("two"){
                  steps{
                      input("Do you want to procceed")
                  }
                }
              stage("Three"){
                when{
                  not{
                     branch "first" 
                  }
                }
                steps{
                  echo "stage three done!!"
                }
              }
            stage("Four"){
              parallel{
                stage("build stage"){
                  steps{
                    echo "unit test done!"
                  }
                }
                stage("test"){
                steps{
                  echo "test done!"
                 }
                }
              }
            }
          }
}
 
