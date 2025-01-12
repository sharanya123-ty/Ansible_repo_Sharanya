pipeline {
    agent { label 'node1' }
    stages {
        stage('Grafana Installation') {
            steps {
                sh '''
                export ANSIBLE_HOST_KEY_CHECKING=False
                ansible-playbook -i /etc/ansible/hosts /opt/Ansible_repo_sharanya/grafana.yml -vv
                '''
            }
        }
    }
}
