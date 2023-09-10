pipeline {
  agent any
  stages {
    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            sh '''#!/bin/bash

((sum=8+1))
echo $sum'''
          }
        }

        stage('Test1') {
          steps {
            echo 'completed'
          }
        }

      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh '''#!/bin/bash
((name="vikas"))
echo $name'''
          }
        }

        stage('Build1') {
          steps {
            echo 'successfully deployed'
          }
        }

      }
    }

    stage('Deploying') {
      steps {
        echo 'Completed'
      }
    }

  }
}