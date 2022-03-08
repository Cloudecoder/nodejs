pipeline { 
  
   agent any

   stages {
   
     stage('Installing Package') { 
        steps { 
           sh 'cd /home/ubuntu && npm -f install' 
        }
     }

      stage("Deploy application") { 
         steps { 
           sh 'cd /home/ubuntu && pm2 -f start server.js'
         }
     }
  
   	}

   }
