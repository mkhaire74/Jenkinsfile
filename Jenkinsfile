pipeline {
    agent any
     parameters
            {
            string (name:'name', defaultValue: 'Jenkins' , description: 'please enter your name')
            choice(name:'Projecttype', choices: 'Maven\nGradle', description: 'select project type')
            booleanParam(name:'display' , defaultValue: true, description: 'do you want to display name and choices on logs')
            }
  
    stages {
        stage('Example') {
            steps {
                script{
              if("${params.display}")
                {
                echo "${params.display}"
                echo "${params.name}"
                echo "${params.Projecttype}"
                }
                }
            }
        }

    }
}
