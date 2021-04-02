pipeline
{
  agent any
    stages
    {
      stage ('Build')
      {
        steps
        {
          echo 'Running Automation Build.'
          sh './gradlew build --no-daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        } // end steps
      } // end stage
    } // end stages
} // end pipeline
