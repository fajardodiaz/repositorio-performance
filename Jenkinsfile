pipeline{
    agent none
    stages{
        stage('Test 1'){
            parallel{
                stage('server-1'){
                    // agent{label 'ubuntu-slave-1'}
                    agent any
                    steps{
                        sh "cd test-servidor-1 && sudo bzt TestJmeter.jmx -report"
                    }
                }
                stage('server-2'){
                    // agent{label 'ubuntu-slave-2'}
                    agent any
                    steps{
                        sh "cd test-servidor-2 && sudo bzt TestJmeter.jmx -report"
                    }
                }
                stage('server-3'){
                    // agent{label 'ubuntu-slave-3'}
                    agent any
                    steps{
                        sh "cd test-servidor-3 && sudo bzt TestJmeter.jmx -report"
                    }
                }
                stage('server-4'){
                    // agent{label 'ubuntu-slave-4'}
                    agent any
                    steps{
                        sh "cd test-servidor-4 && sudo bzt TestJmeter.jmx -report"
                    }
                }
                stage('server-5'){
                    // agent{label 'ubuntu-slave-5'}
                    agent any
                    steps{
                        sh "cd test-servidor-5 && sudo bzt TestJmeter.jmx -report"
                    }
                }
            }
        }
    }
}
