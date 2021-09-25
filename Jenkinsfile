pipeline{
	agent { label 'master' }
	stages {
		stage('BUILD'){
			parallel{
				stage('BUILD1'){
					steps {
						sh 'echo this is my 2nd pipeline job'
						sh 'ls -lrt'		
						sh 'sleep 5'
					}
			}
				stage('BUILD2'){
					steps {
						sh 'echo this is my 2nd pipeline job'
						sh 'head -5'		
						sh 'sleep 5'
					}
			}
		}
	}			
		stage('TEST'){
			steps {
			sh 'echo this is my 2nd pipeline job'
			sh 'du -h'
			}
		}
        }
}
