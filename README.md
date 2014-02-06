mygit
=====

Quickly set up and use Git repos on a private server via SSH. The server acts as the remote and holds bare repos, which the server and clients can easily clone into local working copy repos. The server can be a client too.

server commands:

* `mygit setup` — set up the server by creating a base directory to store all remotes
* `mygit init reponame` — create a repo on the server
* `mygit ffonly reponame true|false` — change `receive.denyNonFastforwards` for a repo on the server
* `mygit remove -f reponame` — remove a repo from the server

client commands:

* `mygit clone reponame` — clone a repo from the server
* `mygit push` — set server as remote for the current local repo
