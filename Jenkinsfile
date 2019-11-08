#!groovy
node('master'){
    stage('Checkout SCM') {
    git 'https://github.com/frank1985/CypressDemo.git'
    }
    stage('Build') {
    bat label: 'Install NPM package', script: 'npm install'
    }
    stage('Test') {
    bat label: 'Run test', script: 'npx cypress run'test
    }
}
