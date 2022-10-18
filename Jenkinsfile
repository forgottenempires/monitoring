pipeline {
    agent any
    stages {
        stage("Verify tooling") {
            steps {
                bat '''
                docker version
                docker info
                docker compose version
                '''
            }
        }
        // stage("Prune Docker data") {
        //     steps {
        //         bat 'docker system prune -a --volumes -f'
        //     }
        // }
        stage("Start containers") {
            steps {
                bat '''
                cd C:/Users/Seda/Desktop/Playground/Monitoring/Prometheus/prometheus-json-exporter-master
                docker-compose up -d
                '''
            }
        }
    }
}