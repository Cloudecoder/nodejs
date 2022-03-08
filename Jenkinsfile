pipeline { 
  
   agent any

   stages {
   
     stage('Installing Package') { 
        steps { 
           cd /home/ubuntu && npm -f install 
        }
     }

      stage("Deploy application") { 
         steps { 
           cd /home/ubuntu && pm2 -f start server.js
         }
     }
  
   	}

   }
