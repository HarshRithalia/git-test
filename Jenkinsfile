pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                    sh """ rm -rf TicketBookingServiceJunitTesting ; git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git """
            }
        }
        stage('install') {
            steps {
                    sh """ mvn clean install -f TicketBookingServiceJunitTesting """
            }
        }
           stage('package') {
            steps {
                   sh """ mvn package -f TicketBookingServiceJunitTesting """
            }
        }
    }
}
