pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'INICIO'
        bat(script: 'echo', label: 'Empezando pipeline...', returnStatus: true)
      }
    }

    stage('Sistema') {
      steps {
        echo 'SISTEMA'
        bat(script: 'echo', label: '%DATE% %TIME%', returnStatus: true)
      }
    }

    stage('Aprobacion') {
      steps {
        input(message: '¿Continuar a FIN?', ok: 'Continuar')
      }
    }

    stage('Fin') {
      steps {
        echo 'FIN'
        echo 'FIN: empezando'
        echo 'FIN: %DATE% %TIME%'
        echo 'FIN: terminado'
      }
    }

  }
}