agent any

    stages {
        stage('Checkout using SOURCE_BRANCH') {

            steps { 
             git branch: 'master', url: 'https://github.com/wakaleo/game-of-life.git'
   }
        }
    stage('checkmarx ast scan') {
     steps { 
        checkmarxASTScanner additionalOptions: '', baseAuthUrl: 'https://ind.iam.checkmarx.net', branchName: 'master', checkmarxInstallation: 'chekmarx Cli', credentialsId: 'Checkmarx_latest_cred', projectName: 'Game-of-life', serverUrl: 'https://ind.ast.checkmarx.net', tenantName: 'kpmg_ast' 
     }
        }
