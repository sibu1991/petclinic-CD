pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'ls -altr'
                        sh 'pwd'
		        sh 'docker pull sibu2272/petclinic:2'
                        sh 'cp -R helm/* .'
		                sh 'ls -altr'
                        sh 'pwd'
                        //sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=registry.hub.docker.com/sibu2272/petclinic --set image.tag=latest'
                        sh '/usr/local/bin/helm upgrade --install --set image.repository="registry.hub.docker.com/sibu2272/petclinic" --set image.tag="2" myjavaapp petclinic/ '

            }           
        }
    }
}
