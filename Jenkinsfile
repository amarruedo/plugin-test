#!groovy

node("macOS-sierra") {
  deleteDir()
  checkout scm
  def vars = gitParams()
  echo vars.commit
  echo vars.shortCommit
  echo vars.buildNumber.toString()

  stage("release" + (vars.release.isPresent ? (vars.release.stage != "" ? "-" + vars.release.stage) : "")){
    if(vars.release.isPresent)
    {
      echo vars.release.version
      echo vars.release.versionNoPrefix
      echo vars.release.versionShort
      echo vars.release.versionShortNoPrefix
    }
  }
}
