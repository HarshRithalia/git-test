pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                    "git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git"
            }
        }
        stage('install') {
            steps {
                    "mvn install -f TicketBookingServiceJunitTesting"
            }
        }
        stage('test') {
            steps {
                    "mvn test -f TicketBookingServiceJunitTesting"
            }
        }
        stage('package') {
            steps {
                    "mvn package -f TicketBookingServiceJunitTesting"
            }
        }
    }
}
