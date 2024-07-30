pipeline 
{
    agent any

    stages 
    {
        stage('Sample Job') 
        {
            steps 
            {
                sh 'mvn test'  // Run Maven tests, for example
            }
        }
        stage('Smoke Test') 
        {
            steps 
            {
                build 'SeleniumTestForFreelanceApplication'
                
            }
        }
         stage('Regression Test') 
        {
            steps 
            {
                build 'SeleniumTestForFreelanceApplicationWithTriggers'
            }
        }
    }
}
