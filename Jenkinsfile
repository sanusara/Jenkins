pipeline {
  agent any
	parameters{
		choice(name: 'VERSION', choices:['1.1.0','1.2.0','1.3.0'],description:'')
		booleanparam(name: 'executetest',defaultValue:true,description:'')
	       }
    stages{
       stage("build"){
		
	steps{
	 echo 'build application...........'
	}

      }
	stage("test"){
	when {
		 expression{
			params.executetest
			}
		   }
	steps{
	 echo 'test application...........'
	}

      }
	stage("Deploy"){
	steps{
	 echo 'Deploy application...........'
	}

      }
}


}

