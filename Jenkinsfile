pipeline {
    agent { label 'node1' }
    stages {
        stage('Grafana Installation') {
            steps {
                sh '''
                export ANSIBLE_HOST_KEY_CHECKING=False
                ansible-playbook -i /etc/ansible/hosts /opt/ansible_roles/grafana.yml -vv
                '''
            }
        }
    }
}
