# Git
>## Abstract
>
>> ### Distributed Version Control System(DVCS)
>>- Use 2 distributed servers
>>> #### Remote server(usually, github)
>>>- Server that stores your projects in repositories. 
>>>- Your main remote server is called *origin*
>>> #### Local server(PC)
>>>- Place where you edit your files of the project. 
- - -
>## commands
> > ### overall
> >- remote to local: clone
> >- in local server: edit code in IDE
> >- local to remote: add - commit - push
> >- git management: status, log
> >- practical usage: branch, checkout, merge, revert, ...
> >- - -
> > ### local to remote
> >>### clone
> >>- clone data of remote server to the local server via URL(HTTPS/SSH). 
> >>
> >>			$ cd ~/dev/dir_u_want # directory where you want to clone
> >>			$ git clone https://github.com/user_name/repo_u_want.git
> >> - - -
> >>### pull
> >>- pull(and merge) recent updates of remote server to the local server
> >>
> >>			$ git pull # pull current branch
> >>			$ git pull origin master # origin server main branch
> >> - - -
> >> ### fetch
> >>- fetch(pull but not merge) recent updates of remote server to the local server
> >>
> >>			$ git fetch
> > - - -
> > ### remote to local
> >>### add
> >>- add file/data to update in *stage*
> >>
> >>			$ git add . # add all modifications of current directory
> >>			$ git add ./source # add all modifications in source directory
> >>			$ git add ./ex01.c # add modification of the file
> >>			$ git add -p # add each with patrol
> >>- - -
> >>### commit
> >>- commit(package) all files/data with message, 
> >>- when modified project is executable(recommended)
> >>
> >>			$ git commit # after this command, should enter a message
> >>			$ 'message for the changes' # 'quotes' to emphasize it's message
> >>- - -
> >>### push
> >>- upload commits to the remote server
> >>
> >>			$ git push origin master # origin server, main branch
> >- - -
> >### management
> >>### status
> >>- check local server's status
> >>- the current location of branch, commitments, modified sources on stage. 
> >>
> >>			$ git status
> >>- - -
> >>### log
> >>- show all commitments
> >>- commitments include [hash, HEAD or not, AUTHOR, message, date]
> >>
> >>			$ git log
> >>			$ git log --graph
> >- - -