pipeline{
        agent any
        stages{
                stage('---clean---'){
                        steps{
                                sh "mvn clean"
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test"
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package"
                        }
                }
                stage('--copy--'){
                        steps{
                                sh "cp /var/lib/jenkins/workspace/Job1/target/movieapp.war /home/contactmarkmuwonge/wildfly-10.1.0.Final/standalone/deployments"
                        }
                }
        }
}
