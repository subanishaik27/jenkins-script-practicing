pipeline{
    agent any
        stages
        {
            stage(build)
            {
                steps
                {
                    echo 'Build App'
                }
            }
            stage(Test)
            {
                steps
                {
                    echo 'Test App'
                }
            }
            stage(Deploy)
            {
                steps
                {
                    echo 'Deploy App'
                }
            }
        }
        post{
            always
            {
                emailext body: 'Summary', subject: 'pipeline status', to: 'subanishaikaws@gmail.com'
            }
            
        }
    }
