node{
	stage('SCM Checkout'){
		git 'https://github.com/harshadgaikwad14/jenkins-example1.git'
	}
	stage('Compile-Package'){
		def mvnHome = tool name: 'apache-maven-3.6.3', type: 'maven'
		sh "${mvnHome}/bin/mvn clean install"
	}
}