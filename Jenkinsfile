pipeline{
	agent any
	tools{
		jdk 'JDK'
		gradle 'Gradle'
		}
	stages{
		stage('Checkout'){
		steps{
		git branch:'master' url:'https://github.com/RashiSaraswat/gradle_test1.git'
		}
		}
		stage('Build'){
		steps{
		sh 'gradle build'
		}
		}
		stage('Test'){
		steps{
		sh 'gradle test'
		}}
		stage('Run Application'){
		steps{
		sh 'gradle run'}
		}
		}
	post{
		success{
			echo 'build and deployment successful'}
		failure{
			echo 'build failure'}
		}
	}
	
		
