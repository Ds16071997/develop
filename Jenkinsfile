pipeline {
    agent { label 'terraform_node1'}
    stages{
        stage (cloning) {
            steps {
             git url:'https://github.com/shopizer-ecommerce/shopizer.git',
             branch : 'master'
        }
    }
        stage (deploying) {
            steps {
                sh 'mvn package'
            }
        }    
}
}