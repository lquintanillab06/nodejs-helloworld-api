pipeline {
	agent any
	tools {nodejs '18.0.0'}
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
