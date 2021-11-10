pipeline{
agent any
         stages
         {
                    stage('Build')
                    {
                       tools {
                              maven 'Maven3.8'
                               }      
                    steps{
                         sh 'mvn --version'    
                         echo"buid the project 111 .."
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
                    
                    stage('Retry')
                     {        
                    steps {
                             retry(4)
                             {
                               echo  " retry test project 111 on server ...."
                               // error " error comment"
                             }
                         }
                     }
                  stage('variable')
                    {
                    steps {
                             script {
                                      def name = "Manak"
                                      if(name == "Manak")
                                      println("Hello ${name}")
                                      else
                                         println("Hoooo")
                                      sleep 2
                                      echo " end of this script"
                                    }  
                            }
                      }
                 }
     }
