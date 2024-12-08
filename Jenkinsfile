node {
    stage('Clone') {
        echo 'Clonage du dépôt...'
        git branch: 'main', url: 'https://github.com/Hedi-Mezghani/jenkins-helloworlds.git'
    }

    stage('Debug') {
        echo 'Vérification de la structure des fichiers...'
        sh 'ls -R'
    }

    stage('Build and Run') {
        echo 'Compilation et exécution...'
        sh '''
        cd jenkins-helloworlds
        javac Main.java
        java Main
        '''
    }
}
