def version
def modifiedFiles
def skipBuild
node{
      stage("check for code change"){
            if (fileExists('app2')){
                  sh 'rm -r app2'
            }
            git credentialsId: 'FaizalGit', url: 'https://github.com/faizalgit/app2'
            sh 'git clone https://github.com/faizalgit/app2'
            sh 'git status'
            sh 'git commit -m'
            scmSkip(deleteBuild: true, skipPattern:'.*\\[skip_build\\].*')
      }
}
