pipeline{
	agent any
	tools{
		gradle'Gradle'
	}
	stages{
		stage('Checkout')
		{
			steps{
				git "https://github.com/Sonupriyankaramesh/gradlebeforetest.git"
			}
		}
		stage('Build')
		{
			steps{
				sh'./gradlew clean build'
			}
		}
		stage('Run Application')
		{
			steps{
				sh'./gradlew run'
			}
		}
	}
}
		
