pipeline{
    agent{
        label "nodejs"
    }
    stages{

	stage("Deploy"){
	   steps{
	     sh '''
		oc project developer-deploy-strategies
		oc start-build greeting-service --follow --wait
	     '''
    }
}
}
}
