pipeline {
	agent any
	tools {nodejs 'nodejs'}
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
