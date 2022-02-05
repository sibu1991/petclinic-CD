pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'ls -altr'
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		                sh 'ls -altr'
                        sh 'pwd'
                        //sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=registry.hub.docker.com/sibu2272/petclinic --set image.tag=latest'
                        sh 'helm upgrade --install --set image.repository="registry.hub.docker.com/sibu2272/petclinic" --set image.tag="1" myjavaapp petclinic/ '
              			
            }           
        }
    }
}