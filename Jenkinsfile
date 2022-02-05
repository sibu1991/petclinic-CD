pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'ls -altr'
                        sh 'pwd'
		        sh 'docker pull sibu2272/newapp'
                        sh 'cp -R helm/* .'
		                sh 'ls -altr'
                        sh 'pwd'
<<<<<<< HEAD
                        //sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=registry.hub.docker.com/sibu2272/petclinic --set image.tag=latest'
                        sh 'helm upgrade --install --set image.repository="registry.hub.docker.com/sibu2272/petclinic" --set image.tag="1" myjavaapp petclinic/ '
=======
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=sibu2272/newapp --set image.tag=1'
>>>>>>> 1d3d554b90a9564db7d7880e442447bc55d0871d
              			
            }           
        }
    }
}
