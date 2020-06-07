//1-->SCRIPTED SYNTAX---OLD ONE
// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('Integration Test') {
// 		echo "Integration Test"
// 	}
// }
//2-->SCRIPTED SYNTAX---OLD ONE--above ones are the same as this one 
//but it wont be as blue boxes as prevoiusly were

// node {
	
// 		echo "Build"
// 		echo "Test"
// 		echo "Integration Test"
// }


//Declarative approach

pipeline {
	agent any
	stages{
		stage('Build'){
			steps{
				echo "Build"
			}
		}

		stage('Test'){
			steps{
				echo "Test"
			}
		}

		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}
	post{
		always{
			echo "I am awesome.. I run always!"
		}
		success{
			echo "I am awesome.. I run Success!"
		}
		failure{
			echo "I am failed.. I run when you fail!"
		}
		//other than above there are other post activity like unstable and changed.
	}
}