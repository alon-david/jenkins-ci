Tweaking to look for the best way to CI with on-premise Jenkins server and hosted GitHub git

curl http://yourserver/git/notifyCommit?url=<URL of the Git repository>[&branches=branch1[,branch2]*][&sha1=<commit ID>]
1. note: in order to activate this we need to activate 'Poll SCM' checkbox
2. best way to post-push hook is the following: git config alias.xpush '!git push $1 $2 && curl http://<server>/git/notifyCommit?url=<repo URL> #' 
