#!groovy

node("master") {
  checkout scm
  def vars = gitVars()
  echo vars.commit
  echo vars.shortCommit
}
