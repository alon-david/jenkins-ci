Tweaking to look for the best way to CI with on-premise Jenkins server and hosted GitHub git

curl http://yourserver/git/notifyCommit?url=<URL of the Git repository>[&branches=branch1[,branch2]*][&sha1=<commit ID>]
note: in order to activate this we need to activate 'Poll SCM' checkbox
