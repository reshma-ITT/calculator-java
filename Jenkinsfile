pipeline {
agent any
stages {
stage ('Compile Stage') {
steps {
withMaven(maven : 'Maven 1') {
sh 'mvn clean compile'
}
}
}
stage ('Testing Stage') {
steps {
withMaven(maven : 'Maven 1') {
sh 'mvn test'
}
}
}
stage ('Install Stage') {
steps {
withMaven(maven : 'Maven 1') {
sh 'mvn install'
}
}
}
}
}