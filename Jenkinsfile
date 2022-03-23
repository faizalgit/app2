def version
def modifiedFiles
node{
      stage("check for code change"){
      git credentialsId: 'FaizalGit', url: 'https://github.com/faizalgit/app2'
      sh 'git clone https://github.com/faizalgit/app2'
      sh 'git status'
      }
}
