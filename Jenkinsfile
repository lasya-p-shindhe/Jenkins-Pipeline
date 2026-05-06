pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compile and package the application source code.'
                echo 'Tool: Maven - a build automation tool used to compile and package Java projects.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Run unit tests to ensure individual code components function correctly.'
                echo 'Task: Run integration tests to ensure all components work together as expected.'
                echo 'Tool: JUnit for unit testing. Selenium for integration testing.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse the code to ensure it meets industry coding standards.'
                echo 'Tool: Checkstyle - a static code analysis tool that checks Java code style and quality.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Perform a security scan to identify known vulnerabilities in the codebase.'
                echo 'Tool: OWASP Dependency-Check - scans project dependencies for known CVEs.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy the application to a staging server for pre-production testing.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 staging instance.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Run integration tests on the staging environment to verify the application works in a production-like setup.'
                echo 'Tool: Selenium WebDriver - automates browser-based integration testing on the staging server.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy the fully tested application to the live production server.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 production instance.'
            }
        }
    }
}
