node{
	stage('SCM Checkout'){
		git 'https://github.com/harshadgaikwad14/jenkins-example1'
	}
	stage('Compile-Package'){
		// following name is getting from http://localhost:8080/job/jenkinsfile-git-maven/pipeline-syntax/
		// Check Video : https://youtu.be/pts8zdHel5E?list=PLH1ul2iNXl7txKuhhDMKenYOThDww6x8S
		def mvnHome = tool name: 'apache-maven-3.6.3', type: 'maven'
		sh "{mvnHome}/bin/mvn clean package"
	}
}