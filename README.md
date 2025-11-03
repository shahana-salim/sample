web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git init
Reinitialized existing Git repository in /home/web/Desktop/prajil/.git/
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git add index.html
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   index.html

web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git config
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry

web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git config --global
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry

web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git config --global user.name "prajil"
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git config --global user.email "prajil@hotmail.com"
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git config --list
user.name=prajil
user.email=prajil@hotmail.com
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git commit -m"added my html file..."
[master (root-commit) f8f03c1] added my html file...
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git status
On branch master
nothing to commit, working tree clean
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (HEAD -> master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git branch style
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git branch script
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git branch --list
* master
  script
  style
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout style
Switched to branch 'style'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (HEAD -> style, script, master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git status
On branch style
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        style.css

nothing added to commit but untracked files present (use "git add" to track)
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git add style.css
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git commit -m"added style"
[style 711fc25] added style
 1 file changed, 3 insertions(+)
 create mode 100644 style.css
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout script
Switched to branch 'script'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git add script
fatal: pathspec 'script' did not match any files
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git add script.js
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git commit -m"script added"
[script 967aaae] script added
 1 file changed, 1 insertion(+)
 create mode 100644 script.js
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log
commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (HEAD -> script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (HEAD -> script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit 711fc25782f5bd713e504453884454fd10dba03a (style)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:29:11 2025 +0530

    added style

commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout 711f
Note: switching to '711f'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 711fc25 added style
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout master
Previous HEAD position was 711fc25 added style
Switched to branch 'master'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout style
Switched to branch 'style'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout style
M       style.css
Already on 'style'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git stash
Saved working directory and index state WIP on style: 711fc25 added style
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
commit 59c0cc9da79e126a550db7ec0bc478eaa1ce21c6 (refs/stash)
Merge: 711fc25 a4a5b49
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    WIP on style: 711fc25 added style

commit a4a5b492a2b59291b7e4e2048e7ff83e3bca9161
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    index on style: 711fc25 added style

commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit 711fc25782f5bd713e504453884454fd10dba03a (HEAD -> style)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:29:11 2025 +0530

    added style

commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
(END)
Merge: 711fc25 a4a5b49
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    WIP on style: 711fc25 added style

commit a4a5b492a2b59291b7e4e2048e7ff83e3bca9161
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    index on style: 711fc25 added style

commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit 711fc25782f5bd713e504453884454fd10dba03a (HEAD -> style)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:29:11 2025 +0530

    added style

commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...
(END)
Merge: 711fc25 a4a5b49
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    WIP on style: 711fc25 added style

commit a4a5b492a2b59291b7e4e2048e7ff83e3bca9161
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    index on style: 711fc25 added style

commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit 711fc25782f5bd713e504453884454fd10dba03a (HEAD -> style)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:29:11 2025 +0530

    added style

commit f8f03c1c70fccff4c7c5049a27feb8fb70f10ba9 (master)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:24:44 2025 +0530

    added my html file...

web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git merge
fatal: No remote for the current branch.
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git merge style
Already up to date.
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout master
Switched to branch 'master'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git merge style
Updating f8f03c1..711fc25
Fast-forward
 style.css | 3 +++
 1 file changed, 3 insertions(+)
 create mode 100644 style.css
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git merge script
Merge made by the 'ort' strategy.
 script.js | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 script.js
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git log --all
commit 51548fe5a7db04a30d90f9dac9885ea2ff4eaf04 (HEAD -> master)
Merge: 711fc25 967aaae
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:36:58 2025 +0530

    Merge branch 'script'

commit 59c0cc9da79e126a550db7ec0bc478eaa1ce21c6 (refs/stash)
Merge: 711fc25 a4a5b49
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    WIP on style: 711fc25 added style

commit a4a5b492a2b59291b7e4e2048e7ff83e3bca9161
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:34:37 2025 +0530

    index on style: 711fc25 added style

commit 967aaae6b98238ecd1a39143162f711e9d4ff269 (script)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:31:05 2025 +0530

    script added

commit 711fc25782f5bd713e504453884454fd10dba03a (style)
Author: prajil <prajil@hotmail.com>
Date:   Mon Nov 3 11:29:11 2025 +0530
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout 59c0cc9da79e126a550db7ec0bc478eaa1ce21c6
Note: switching to '59c0cc9da79e126a550db7ec0bc478eaa1ce21c6'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 59c0cc9 WIP on style: 711fc25 added style
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git checkout master
Previous HEAD position was 59c0cc9 WIP on style: 711fc25 added style
Switched to branch 'master'
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ git clone https://github.com/shahana-salim/sample.git
Cloning into 'sample'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil$ cd sample
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ ls
index.html  README.md  script.js  style.css
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js
        style.css

nothing added to commit but untracked files present (use "git add" to track)
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git add .
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git commit -m"added a website"
[main 26627c6] added a website
 3 files changed, 15 insertions(+)
 create mode 100644 index.html
 create mode 100644 script.js
 create mode 100644 style.css
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git remote add hub https://github.com/shahana-salim/sample.git
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git remote
hub
origin
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git branch 
* main
web@softlab-OptiPlex-5055-Ryzen-CPU:~/Desktop/prajil/sample$ git push hub main
