pipeline {
	agent any
	stages {
		stage(‘Upload to AWS’) {
        steps {
          withAWS(region:’eu-north-1b’,credentials:’was-static’) {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true,		file:’index.html’, bucket:’jenkins-hosting’)
				}
			      }
			    }
			  }
