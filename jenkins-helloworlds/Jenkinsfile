node {
    stage('Clone') {
        git 'https://github.com/Hedi-Mezghani/jenkins-helloworlds.git'
    }

    stage('Debug') {
        // Lister les fichiers pour vérifier leur emplacement
        sh 'ls -R'
    }

    stage('Build and Run') {
        // Compilation et exécution dans le bon répertoire
        sh '''
        cd jenkins-helloworlds
        javac Main.java
        java Main
        '''
    }
}
