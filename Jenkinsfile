pipeline {
    agent any
    tools {
        maven 'Maven-3.9.9'  // 与你在全局工具配置中设置的名称一致
        jdk 'JDK21'          // 确保也配置了JDK
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}