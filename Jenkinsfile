pipeline{
agent any
         stages
         {
                    stage('Buid')
                    {
                    steps{
                         echo"buid the project 111 ...."
                         }
                    }
                    
                   stage('Test')
                    {
                    steps{
                         echo"Test the project 111 and share the result...."
                         }
                    }
                    
                    stage('Deploy')
                    {
                    steps{
                         echo"Deply the result of project 111 on server ...."
                         }
                    }
                  stage('variable')
                    {
                    steps {
                             script {
                                      def name = "Manak"
                                      if(name == "Manak")
                                         println("HEllo $(name)")
                                      else
                                         println("Hoooo")
                                      sleep 2
                                      echo " end of this script"
                                   }  
                             }
                         }
                    }
          }
