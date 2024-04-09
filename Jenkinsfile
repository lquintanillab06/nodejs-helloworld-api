pipeline {
	agent any
	tools {nodejs '21.7.1'}
	stages{
		stage('Instalando dependencias'){
			steps {
				sh 'npm install'
			}
		}
		stage('testing'){
			steps{
				sh 'npm test'
			}
		}
	}
	post{
		success{
			echo 'Deployment terminado exitosamente'
		}
		failure{
			echo 'Fallo'
		}
	}
}
