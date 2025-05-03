def call(Map config = [:]) {
    def mvnCmd = config.get('mavenCmd', 'mvn clean install')

    echo "Running Maven Command: ${mvnCmd}"
    sh mvnCmd
}
