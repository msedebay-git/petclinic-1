pipeline {
	agent any
    stages {
        stage('Build on k8s cluster ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --uninstall petclinic-app petclinic  --set image.repository=registry.hub.docker.com/msedebaydockerhub/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
