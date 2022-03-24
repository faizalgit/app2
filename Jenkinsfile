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
            item = hudson.model.Hudson.instance.getItem("app2_pipeline")
            build = item.getLastBuild()
            echo 'build time'
            println build.getTime()
      }
        
}
