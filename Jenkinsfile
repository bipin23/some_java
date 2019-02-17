node  {
  cleanWs()     
     stage('SCM checkout')     
                {        
 		   checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/bipin23/some_java']]]
		 }    
    stage('Build Stage')    
        {        
	echo "hello build"    
	}
post {
	always {
		echo 'I will always say Hello again'
	}
}	
}	
