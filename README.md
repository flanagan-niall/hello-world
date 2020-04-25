# hello-world
I edited this!

# Configuring Git for VS Code.
    -> Use SSH to avoid need to authenticate for every pull/push
    -> Setup Git account
    -> Setup Git repo

    On Pi:
    -> Install Git (probably already installed) - $ sudo apt install git
    -> Setup account details -$ git config --global user.name "YourGitHubUsername"
                              $ git config --global user.email "yourgithub@email.com"

    -> VS Code needs this - $ sudo apt install ssh-askpass
    -> Generate ssh key - $ ssh-keygen -t rsa -C "yourgithub@email.com"
    -> Copy key to clipboard
    
    On Git:
    -> Add key - Setting - SSH and GPG keys - add SSh Key

    On Pi:
    -> Add Git to known hosts - $ ssh-keyscan -t rsa github.com > ~/.ssh/known_hosts

    On Git:
    -> Clone repo using SSH url

    On Pi:
    -> Clone repo - ctrl + shift + p - Git: Clone
    -> paste SSH url


    GTG!

# Configuring Git to ignore files.
    -> In the root of your repo edit .git/info/exclude
        e.g. .pyc will ignore all pyc files from scm