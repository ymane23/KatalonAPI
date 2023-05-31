pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat """
                cd  C:\\Tools\\Katalon_Studio_Engine_Windows_64-8.6.0\\Katalon_Studio_Engine_Windows_64-8.6.0
                katalonc -noSplash -runMode=console -projectPath="C:\\Users\\ymane\\.jenkins\\workspace\\Katalon_API\\KatalonAPI.prj" -retry=0 -testSuitePath="Test Suites/Scripts" -browserType="Chrome" -executionProfile="default" -apiKey="b93d677f-7391-4be2-b933-695533c6333c" --config -proxy.auth.option=NO_PROXY -proxy.system.option=NO_PROXY -proxy.system.applyToDesiredCapabilities=true
                """

            }
        }
        stage('Test') {
            steps {
                bat """
                cd  C:\\Tools\\Katalon_Studio_Engine_Windows_64-8.6.0\\Katalon_Studio_Engine_Windows_64-8.6.0
                katalonc -noSplash -runMode=console -projectPath="C:\\Users\\ymane\\.jenkins\\workspace\\Katalon_API\\KatalonAPI.prj" -retry=0 -testSuitePath="Test Suites/Scripts" -browserType="Chrome" -executionProfile="default" -apiKey="b93d677f-7391-4be2-b933-695533c6333c" --config -proxy.auth.option=NO_PROXY -proxy.system.option=NO_PROXY -proxy.system.applyToDesiredCapabilities=true
                """

            }
        }

    }

}
