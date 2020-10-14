library 'jenkins_shared'

pipeline {
    agent { label 'integration' }
    parameters {
        string(defaultValue: "PCK.AUTOMIC_MICROSOFT_OFFICE365", description: 'Package Name', name: 'package_name')
        string(defaultValue: "Package.MICROSOFT.OFFICE365", description: 'lifecycleentity_name', name: 'lifecycleentity_name')
        string(defaultValue: "package.microsoft.office365", description: 'le_name_lowercase', name: 'le_name_lowercase')
        string(defaultValue: "pck_microsoft_office365", description: 'le_technical_name', name: 'le_technical_name')
        string(defaultValue: "pck.automic_microsoft_office365", description: 'component_name', name: 'component_name')
      	string(defaultValue: "packages/$params.package_name", description: 'repository name', name: 'repo_name')
        string(defaultValue: "pck.automic_microsoft_office365.test", description: 'Pack Test Name', name: 'pck_test_name')
    }
    stages {
        stage('Build ActionPack') {
            steps {
                buildParameters()
                script {
                    env.tool_dir=""
                    env.source_dir="ae"
                    env.require_packs="PCK.AUTOMIC_BOND"
                }
                apBuildTemplate()
            }              
        }
		
		stage('Release ActionPack') {
			when { 
			    expression { return env.branch_type == 'release' }
			}
            steps {
                apReleaseTemplate()
            }       
                   
        }
    }
}
