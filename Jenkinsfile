node('master') {
    stage("Fetch Source Code") {
        git 'https://github.com/nadsrice/lesson5'
    }
    dir('') {
        printMessage('Running Pipeline')

        stage("Testing") {
            sh 'python test_functions.py'
        }

        printMessage('Pipeline Complete')
    }
}

def printMessage(message) {
    echo "${message}"
}