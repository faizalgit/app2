def version
def modifiedFiles
node{
      stage("check for code change"){
            if (filexist('app2')){
                  sh 'rm -r app2'
            }
            git credentialsId: 'FaizalGit', url: 'https://github.com/faizalgit/app2'
            sh 'git clone https://github.com/faizalgit/app2'
            sh 'git status'
            sh 'git commit -m "skip_build"'
      }
}
