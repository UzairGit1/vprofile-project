Pipeline {
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK8"
    }
    envirnoment {
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'admin123'
        CENTRAL_REPO = 'vprofile-maven-central'
        RELEASE_REPO = 'vprofile-release'
        SNAP_REPO = 'vprofile-snapshot'
        NEXUS_GRP_REPO = 'vpro-maven-repo'
        NEXUSIP = '172.31.87.31'
        NEXUS_PORT = '8081'
        NEXUS_LOGIN = 'nexuslogin'
    }
    stages {
        stage('Build'){
            steps{
                sh 'mvn -install -DskipTests -s settings.xml'
            }
        }
    }
}