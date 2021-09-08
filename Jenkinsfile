pipeline {
	agent { node { label "master" } }
		
	stages {
		stage('Deploy To DEV') {
			steps {
			    script {
				    sh """#!/bin/bash
					    set -exf
						if [ "${Path}" = "dags" ]
						then
						    echo "dags"
						elif [ "${Path}" = "configs" ]
						then
						    echo "config"
						elif [ "${Path}" = "utils" ]
						then
							echo "utils"
						elif [ "${Path}" = "ingestion" ]
						then
							echo "ingestion"
						else
						then
						    echo "all changes are made"
						fi
                    """
				 }
			}
		}
	}
}
