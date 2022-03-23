def version
def modifiedFiles
def skipBuild
node{
      stage("check for code change"){
            if (fileExists('app2')){
                  sh 'rm -r app2'
            }
            git credentialsId: 'FaizalGit', url: 'https://github.com/faizalgit/app2'
            sh 'git checkout master'
            sh 'git clone https://github.com/faizalgit/app2'
            sh 'git status'
            sh 'git add *'
            sh 'git commit -m "skip_build"'
            scmSkip(deleteBuild: true, skipPattern:'.*\\[skip_build\\].*')
      }
      stage("Compile"){
            echo 'i am in compile stage'
      }      
}
