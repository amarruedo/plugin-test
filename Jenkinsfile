#!groovy

node("macOS-sierra") {
  checkout scm
  def vars = gitVars()
  echo vars.commit
  echo vars.shortCommit
  echo vars.buildNumber.toString()

  if(vars.release.isPresent)
  {
    echo vars.release.version
    echo vars.release.versionNoPrefix
    echo vars.release.versionShort
    echo vars.release.versionShortNoPrefix
  }
}
