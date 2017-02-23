#!groovy

node("master") {
  checkout scm
  def vars = gitVars()
  echo vars.commit
  echo vars.shortCommit
  echo vars.buildNumber.toString()

  if(vars.release.isPresent)
  {
    echo vars.release.version
  }
}
