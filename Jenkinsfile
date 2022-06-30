pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                    sh """ git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git """
            }
        }
        stage('install') {
            steps {
                    sh """ mvn install -f TicketBookingServiceJunitTesting """
            }
        }
           stage('package') {
            steps {
                   sh """ mvn package -f TicketBookingServiceJunitTesting """
            }
        }
    }
}
