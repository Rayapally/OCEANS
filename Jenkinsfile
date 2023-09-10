pipeline {
  agent any
  stages {
    stage('TEST') {
      steps {
        sh '''#!/bin/bash

((sum=8+1))
echo $sum'''
      }
    }

    stage('Build') {
      steps {
        sh '''#!/bin/bash
((name="vikas"))
echo $name'''
      }
    }

    stage('Deploying') {
      steps {
        echo 'Completed'
      }
    }

  }
}