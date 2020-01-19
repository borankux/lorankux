pipeline {
  agent any
  stages {
    stage('PreBuild') {
      steps {
        sh '/Users/mablat/composer/composer install'
        sh './vendor/bin/phpunit'
        sh '/usr/local/bin/terminal-notifier -title ProjectX -subtitle "Prebuilt" -message "Build Successfull" -appIcon /Users/mablat/.jenkins/resources/success.png'
      }
    }

  }
}