node("vagrant") {
    docker.image('maven:3.5.2-jdk-8').inside {
        withMaven() {
            git "https://github.com/takari/maven-wrapper.git"
            sh 'export PATH=$MVN_CMD_DIR:$PATH && which mvn && env && mvn help:effective-settings'
        }
    }
}
