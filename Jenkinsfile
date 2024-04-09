pipeline {
	agent any
	stages{
		stage('Instalando dependencias'){
			steps {
				sh 'nvm use 18.0.0'
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
