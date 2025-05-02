pipeline {
agent any
tools {
maven "maven'

stages {
stage ("Clean up"){
steps {
deleteDir()

1

}
Stage ("Clone repo"){
steps {
sh "git clone https://github.com/MaBouz/exp1-spring.git"

stage ("Generate backend image") {
steps {
dir("expi-spring"){
sh "mvn clean install"
sh "docker build -t docexp1-spring ."

Stage ("Run docker compose") {
steps {
dir("expi-spring"){
sh " docker compose up -d"
