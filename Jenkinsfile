pipeline{
  agent any
  parameters{
        choice(name: 'action', choices: 'create\ndelete', description: 'Choose to create/Destroy')
  }
   stages{
     stage('Git Checkout'){
       steps{
         echo "Git Checkout"
       }
     }
     stage('build'){
       when { expression {  params.action == 'create' } }
       steps{
         echo "Creating the application..."
       }
       
     }
     
   }
}
