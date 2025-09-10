pipeline {
  agent any

  stages {
    stage('Pinging') {
      steps {
        echo "Jenkins is connected to 'SIT753-8_1C-pipeline'"
      }
    }

    stage('Stage-1-Build') {
      steps {
        echo "Stage 1: Build"
        echo "Task: Compile the source code and package it into an artifact for testing."
        echo "Tool: Maven"
      }
    }

    stage('Stage-2-Unit and Integration Tests') {
      steps {
        echo "Stage 2: Unit and Integration Tests"
        echo "Task: Run unit tests for small pieces of code and integration tests to check modules work together."
        echo "Tool: JUnit"
      }
    }

    stage('Stage-3-Code Analysis') {
      steps {
        echo "Stage 3: Code Analysis"
        echo "Task: Scan the code for style problems, maintainability, and coding standards."
        echo "Tool: SonarQube"
      }
    }

    stage('Stage-4-Security Scan') {
      steps {
        echo "Stage 4: Security Scan"
        echo "Task: Perform a security scan on the code and dependencies to find vulnerabilities."
        echo "Tool: OWASP Dependency-Check"
      }
    }

    stage('Stage-5-Deploy to Staging') {
      steps {
        echo "Stage 5: Deploy to Staging"
        echo "Task: Deploy the application to a staging environment that mimics production."
        echo "Tool: Docker"
      }
    }

    stage('Stage-6-Integration Tests on Staging') {
      steps {
        echo "Stage 6: Integration Tests on Staging"
        echo "Task: Run integration tests on staging to confirm the app works outside the dev machine."
        echo "Tool: Selenium"
      }
    }

    stage('Stage-7-Deploy to Production') {
      steps {
        echo "Stage 7: Deploy to Production"
        echo "Task: Push the final tested build into the production environment for real users."
        echo "Tool: Ansible"
      }
    }
  }
}

