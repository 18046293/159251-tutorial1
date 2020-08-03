This is the command line history for setting up the repository


C:\Users\18046293>git config
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [value-regex]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex]
    --unset-all           remove all matches: name [value-regex]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry


C:\Users\18046293>git config --global user.name "David Schoeman"

C:\Users\18046293>git config --global user.email david@rurunz.co.nz

C:\Users\18046293>git init
Initialized empty Git repository in C:/Users/18046293/.git/

C:\Users\18046293>cd C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -am "My first try with Git repository"
[master 8603b4a] My first try with Git repository
 6 files changed, 4 insertions(+), 1 deletion(-)
 create mode 100644 .DS_Store
 mode change 100755 => 100644 HelloWorldInCpp.cpp
 mode change 100755 => 100644 README.txt
 mode change 100755 => 100644 Simplecalculator.py
 mode change 100755 => 100644 leapYear.java
 mode change 100755 => 100644 leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch Branch-test

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout Branch-test
Switched to branch 'Branch-test'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.java

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .java
fatal: pathspec '.java' did not match any files

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch SecondBranch

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout SecondBranch
Switched to branch 'SecondBranch'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.txt

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.cpp

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge SecondBranch
Already up to date.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge Branch-test
Already up to date.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- Branch-test

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- SecondBranch
fatal: A branch named 'd-' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-SecondBranch

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
fatal: A branch named 'd-' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
Author: David Schoeman <david@rurunz.co.nz>
Date:   Mon Aug 3 21:04:57 2020 +1200

    My first try with Git repository

commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
Author: Amjed Tahir <A.Tahir@massey.ac.nz>
Date:   Mon Jul 22 09:22:11 2019 +1200

    changed

commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
Author: Amjed Tahir <A.Tahir@massey.ac.nz>
Date:   Mon Jul 22 09:15:55 2019 +1200

    first commit

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch -all
error: did you mean `--all` (with two dashes)?

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show -branch -all
error: switch `l' expects a numerical value

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show
commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
Author: David Schoeman <david@rurunz.co.nz>
Date:   Mon Aug 3 21:04:57 2020 +1200

    My first try with Git repository

diff --git a/.DS_Store b/.DS_Store
new file mode 100644
index 0000000..5008ddf
Binary files /dev/null and b/.DS_Store differ
diff --git a/HelloWorldInCpp.cpp b/HelloWorldInCpp.cpp
old mode 100755
new mode 100644
diff --git a/README.txt b/README.txt
old mode 100755
new mode 100644
diff --git a/Simplecalculator.py b/Simplecalculator.py
old mode 100755
new mode 100644
diff --git a/leapYear.java b/leapYear.java
old mode 100755
new mode 100644
diff --git a/leapYear.py b/leapYear.py
old mode 100755
new mode 100644
index 83a3b28..62117ae
--- a/leapYear.py
+++ b/leapYear.py
@@ -4,10 +4,13 @@
 year = int(input("Enter a year: "))
 if (year % 4) == 0:
    if (year % 100) == 0:
-       if (year % 400) == 0:           print("{0} is a leap year".format(year))
+       if (year % 400) == 0:^M
+           print("{0} is a leap year".format(year))^M
        else:
            print("{0} is not a leap year".format(year))
    else:
        print("{0} is a leap year".format(year))
 else:
    print("{0} is not a leap year".format(year))
+^M
+print("done")^M

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch
  Branch-test
* SecondBranch
  d-
  d-Branch-test
  d-SecondBranch
  master

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch master
fatal: A branch named 'master' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
Switched to branch 'master'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
fatal: A branch named 'd-' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test
fatal: A branch named 'd-Branch-test' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- d-Branch-test
fatal: A branch named 'd-' already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-Branch-test
Deleted branch d-Branch-test (was 8603b4a).

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-
Deleted branch d- (was 8603b4a).

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-SecondBranch
Deleted branch d-SecondBranch (was 8603b4a).

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch
! [Branch-test] My first try with Git repository
 ! [SecondBranch] My first try with Git repository
  * [master] My first try with Git repository
---
++* [Branch-test] My first try with Git repository

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch --all
! [Branch-test] My first try with Git repository
 ! [SecondBranch] My first try with Git repository
  * [master] My first try with Git repository
---
++* [Branch-test] My first try with Git repository

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git check-out master
git: 'check-out' is not a git command. See 'git --help'.

The most similar command is
        checkout

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
Already on 'master'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git ls-tree -r master --name-only
.DS_Store
HelloWorldInCpp.cpp
README.txt
Simplecalculator.py
leapYear.java
leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch feature-2

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
Switched to branch 'feature-2'
M       leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git diff leapYear.py
diff --git a/leapYear.py b/leapYear.py
index 62117ae..466671e 100644
--- a/leapYear.py
+++ b/leapYear.py
@@ -13,4 +13,4 @@ if (year % 4) == 0:
 else:
    print("{0} is not a leap year".format(year))

-print("done")
+

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -m "changed leapYear.py"
[feature-2 d244b0d] changed leapYear.py
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
Switched to branch 'master'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
fatal: No remote for the current branch.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
Switched to branch 'feature-2'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
fatal: No remote for the current branch.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
Switched to branch 'master'

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge feature-2
Updating 8603b4a..d244b0d
Fast-forward
 leapYear.py | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log --all --oneline --graph --decorate
* d244b0d (HEAD -> master, feature-2) changed leapYear.py
* 8603b4a (SecondBranch, Branch-test) My first try with Git repository
* 68892c4 changed
* 5b1a3fe first commit

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /help
fatal: '/help' is not a valid tag name.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /?
fatal: '/?' is not a valid tag name.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git /?
git: '/?' is not a git command. See 'git --help'.

The most similar commands are
        am
        gc
        mv
        p4
        rm

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag help

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -d help
Deleted tag 'help' (was d244b0d)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear
unknown option: -a
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://github.com/18046293/159251-tutorial1.git

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 2 threads
Compressing objects: 100% (17/17), done.
Writing objects: 100% (17/17), 2.14 KiB | 548.00 KiB/s, done.
Total 17 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), done.
To https://github.com/18046293/159251-tutorial1.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/18046293/159251-tutorial1.git
 * [new branch]      Branch-test -> Branch-test
 * [new branch]      SecondBranch -> SecondBranch
 * [new branch]      feature-2 -> feature-2
Branch 'master' set up to track remote branch 'master' from 'origin'.
Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push origin --tags
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 203 bytes | 203.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/18046293/159251-tutorial1.git
 * [new tag]         leapYear -> leapYear

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
fatal: remote origin already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
Everything up-to-date
Branch 'master' set up to track remote branch 'master' from 'origin'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin -all
error: did you mean `--all` (with two dashes)?

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
Everything up-to-date
Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
Branch 'master' set up to track remote branch 'master' from 'origin'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
fatal: remote origin already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
fatal: remote origin already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
fatal: remote origin already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
fatal: remote origin already exists.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
Everything up-to-date
Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
Branch 'master' set up to track remote branch 'master' from 'origin'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
commit d244b0d2580f66cfc635914311d727a2ea1d31b5 (HEAD -> master, tag: leapYear, origin/feature-2, feature-2)
Author: David Schoeman <david@rurunz.co.nz>
Date:   Mon Aug 3 21:27:42 2020 +1200

    changed leapYear.py

commit 8603b4a2f7741755e146620770dc8adf89792feb (origin/SecondBranch, origin/Branch-test, SecondBranch, Branch-test)
Author: David Schoeman <david@rurunz.co.nz>
Date:   Mon Aug 3 21:04:57 2020 +1200

    My first try with Git repository

commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
Author: Amjed Tahir <A.Tahir@massey.ac.nz>
Date:   Mon Jul 22 09:22:11 2019 +1200

    changed

commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
Author: Amjed Tahir <A.Tahir@massey.ac.nz>
Date:   Mon Jul 22 09:15:55 2019 +1200

    first commit

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git hist
git: 'hist' is not a git command. See 'git --help'.

The most similar command is
        bisect

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git --help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git status
On branch master
Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git statusC:\Users\18046293>git config
git: 'statusC:\Users\18046293' is not a git command. See 'git --help'.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git config [<options>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Config file location
'Config' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --global              use global config file
'--global' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --system              use system config file
'--system' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --local               use repository config file
'--local' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --worktree            use per-worktree config file
'--worktree' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -f, --file <file>     use given config file
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --blob <blob-id>      read config from given blob object
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Action
'Action' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get                 get value: name [value-regex]
'--get' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-all             get all values: key [value-regex]
'--get-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-regexp          get values for regexp: name-regex [value-regex]
'--get-regexp' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-urlmatch        get value specific for the URL: section[.var] URL
'--get-urlmatch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --replace-all         replace all matching variables: name value [value_regex]
'--replace-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --add                 add a new variable: name value
'--add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --unset               remove a variable: name [value-regex]
'--unset' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --unset-all           remove all matches: name [value-regex]
'--unset-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --rename-section      rename section: old-name new-name
'--rename-section' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --remove-section      remove a section: name
'--remove-section' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -l, --list            list all
'-l' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -e, --edit            open an editor
'-e' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-color           find the color configured: slot [default]
'--get-color' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-colorbool       find the color setting: slot [stdout-is-tty]
'--get-colorbool' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Type
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -t, --type <>         value is given this type
> was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --bool                value is "true" or "false"
'--bool' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --int                 value is decimal number
'--int' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --bool-or-int         value is --bool or --int
'--bool-or-int' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --path                value is a path (file or directory name)
'--path' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --expiry-date         value is an expiry date
'--expiry-date' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Other
'Other' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -z, --null            terminate values with NUL byte
'-z' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --name-only           show variable names only
'--name-only' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --includes            respect include directives on lookup
'--includes' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --show-origin         show origin of config (file, standard input, blob, command line)
'--show-origin' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --show-scope          show scope of config (worktree, local, global, system, command)
'--show-scope' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --default <value>     with --get, use default value when missing entry
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git config --global user.name "David Schoeman"
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git config --global user.email david@rurunz.co.nz
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git init
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Initialized empty Git repository in C:/Users/18046293/.git/
'Initialized' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>cd C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -am "My first try with Git repository"
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>[master 8603b4a] My first try with Git repository
'[master' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 6 files changed, 4 insertions(+), 1 deletion(-)
'6' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> create mode 100644 .DS_Store
'create' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 HelloWorldInCpp.cpp

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 README.txt

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 Simplecalculator.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 leapYear.java

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'Branch-test'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.java
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .java
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: pathspec '.java' did not match any files
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'SecondBranch'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.txt
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.cpp
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already up to date.
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already up to date.
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:22:11 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:15:55 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    first commit
'first' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: did you mean `--all` (with two dashes)?
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show -branch -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: switch `l' expects a numerical value
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/.DS_Store b/.DS_Store
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new file mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 0000000..5008ddf
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Binary files /dev/null and b/.DS_Store differ
'Binary' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/HelloWorldInCpp.cpp b/HelloWorldInCpp.cpp
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/README.txt b/README.txt
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/Simplecalculator.py b/Simplecalculator.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.java b/leapYear.java
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.py b/leapYear.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 83a3b28..62117ae
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>--- a/leapYear.py
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+++ b/leapYear.py
'+++' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>@@ -4,10 +4,13 @@
'-4' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> year = int(input("Enter a year: "))
'year' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> if (year % 4) == 0:
% was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    if (year % 100) == 0:
% was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>-       if (year % 400) == 0:           print("{0} is a leap year".format(year))
'-' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+       if (year % 400) == 0:^M
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+           print("{0} is a leap year".format(year))^M
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>            print("{0} is not a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        print("{0} is a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    print("{0} is not a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+^M
'+M' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+print("done")^M
'+print' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>These are common Git commands used in various situations:
'These' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>start a working area (see also: git help tutorial)
The system cannot find the file a.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   clone             Clone a repository into a new directory
'clone' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   init              Create an empty Git repository or reinitialize an existing one
'init' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>work on the current change (see also: git help everyday)
'work' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   add               Add file contents to the index
'add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   mv                Move or rename a file, a directory, or a symlink
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   restore           Restore working tree files
'restore' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rm                Remove files from the working tree and from the index
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   sparse-checkout   Initialize and modify the sparse-checkout
'sparse-checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>examine the history and state (see also: git help revisions)
'examine' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   bisect            Use binary search to find the commit that introduced a bug
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   diff              Show changes between commits, commit and working tree, etc
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   grep              Print lines matching a pattern
'grep' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   log               Show commit logs
'log' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   show              Show various types of objects
'show' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   status            Show the working tree status
'status' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>grow, mark and tweak your common history
'grow' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   branch            List, create, or delete branches
'branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   commit            Record changes to the repository
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   merge             Join two or more development histories together
'merge' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rebase            Reapply commits on top of another base tip
'rebase' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   reset             Reset current HEAD to the specified state
Invalid parameter(s)
RESET { SESSION }

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   switch            Switch branches
'switch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   tag               Create, list, delete or verify a tag object signed with GPG
'tag' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>collaborate (see also: git help workflows)
'collaborate' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   fetch             Download objects and refs from another repository
'fetch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   pull              Fetch from and integrate with another repository or a local branch
'pull' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   push              Update remote refs along with associated objects
'push' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>'git help -a' and 'git help -g' list available subcommands and some
''git' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>concept guides. See 'git help <command>' or 'git help <concept>'
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>to read about a specific subcommand or concept.
'to' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>See 'git help git' for an overview of the system.
'See' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  Branch-test
'Branch-test' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* SecondBranch
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-
'd-' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-Branch-test
'd-Branch-test' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-SecondBranch
'd-SecondBranch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  master
'master' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'master' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-Branch-test' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d-Branch-test (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d- (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d-SecondBranch (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>! [Branch-test] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> ! [SecondBranch] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  * [master] My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>---
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>++* [Branch-test] My first try with Git repository
'++*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>! [Branch-test] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> ! [SecondBranch] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  * [master] My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>---
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>++* [Branch-test] My first try with Git repository
'++*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git check-out master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: 'check-out' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar command is
'The' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        checkout
'checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already on 'master'
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git ls-tree -r master --name-only
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>.DS_Store

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>HelloWorldInCpp.cpp

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>README.txt

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Simplecalculator.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>leapYear.java

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'feature-2'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>M       leapYear.py
'M' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git diff leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.py b/leapYear.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 62117ae..466671e 100644
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>--- a/leapYear.py
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+++ b/leapYear.py
'+++' is not recognized as an internal or external command,
operable program or batch file.


C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>@@ -13,4 +13,4 @@ if (year % 4) == 0:
'-13' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    print("{0} is not a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>-print("done")
'-print' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -m "changed leapYear.py"
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>[feature-2 d244b0d] changed leapYear.py
'[feature-2' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 1 file changed, 1 insertion(+), 1 deletion(-)
'1' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: No remote for the current branch.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'feature-2'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: No remote for the current branch.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Updating 8603b4a..d244b0d
'Updating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Fast-forward
'Fast-forward' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> leapYear.py | 2 +-
'2' is not recognized as an internal or external command,
operable program or batch file.


C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 1 file changed, 1 insertion(+), 1 deletion(-)
'1' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log --all --oneline --graph --decorate
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* d244b0d (HEAD -> master, feature-2) changed leapYear.py
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 8603b4a (SecondBranch, Branch-test) My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 68892c4 changed
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 5b1a3fe first commit
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: '/help' is not a valid tag name.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /?
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: '/?' is not a valid tag name.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git /?
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: '/?' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar commands are
'The' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        am
'am' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        gc
'gc' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        mv
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        p4
'p4' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        rm
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -d help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted tag 'help' (was d244b0d)
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>unknown option: -a
'unknown' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://github.com/18046293/159251-tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Enumerating objects: 17, done.
'Enumerating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Counting objects: 100% (17/17), done.
'Counting' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Delta compression using up to 2 threads
'Delta' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Compressing objects: 100% (17/17), done.
'Compressing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Writing objects: 100% (17/17), 2.14 KiB | 548.00 KiB/s, done.
'Writing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 17 (delta 6), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>remote: Resolving deltas: 100% (6/6), done.
'remote:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      master -> master
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      Branch-test -> Branch-test
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      SecondBranch -> SecondBranch
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      feature-2 -> feature-2
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push origin --tags
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Enumerating objects: 1, done.
'Enumerating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Counting objects: 100% (1/1), done.
'Counting' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Writing objects: 100% (1/1), 203 bytes | 203.00 KiB/s, done.
'Writing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new tag]         leapYear -> leapYear
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: did you mean `--all` (with two dashes)?
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit d244b0d2580f66cfc635914311d727a2ea1d31b5 (HEAD -> master, tag: leapYear, origin/feature-2, feature-2)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:27:42 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed leapYear.py
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (origin/SecondBranch, origin/Branch-test, SecondBranch, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:22:11 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:15:55 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    first commit
'first' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git hist
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: 'hist' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar command is
'The' is not recognized as an internal or external command,
operable program or batch file.
[main 2020-08-03T10:36:06.542Z] update#setState idle

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        bisect
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git --help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>These are common Git commands used in various situations:
'These' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>start a working area (see also: git help tutorial)
(node:2400) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:2400) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:5984) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:5984) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:2400) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:2400) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
The system cannot find the file a.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   clone             Clone a repository into a new directory
'clone' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   init              Create an empty Git repository or reinitialize an existing one
'init' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>work on the current change (see also: git help everyday)
'work' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   add               Add file contents to the index
'add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   mv                Move or rename a file, a directory, or a symlink
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   restore           Restore working tree files
'restore' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rm                Remove files from the working tree and from the index
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   sparse-checkout   Initialize and modify the sparse-checkout
'sparse-checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>examine the history and state (see also: git help revisions)
'examine' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   bisect            Use binary search to find the commit that introduced a bug
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   diff              Show changes between commits, commit and working tree, etc
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   grep              Print lines matching a pattern
'grep' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   log               Show commit logs
'log' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   show              Show various types of objects
'show' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   status            Show the working tree status
'status' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>grow, mark and tweak your common history
'grow' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   branch            List, create, or delete branches
'branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   commit            Record changes to the repository
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   merge             Join two or more development histories together
'merge' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rebase            Reapply commits on top of another base tip
'rebase' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   reset             Reset current HEAD to the specified state
Invalid parameter(s)
RESET { SESSION }

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   switch            Switch branches
'switch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   tag               Create, list, delete or verify a tag object signed with GPG
'tag' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>collaborate (see also: git help workflows)
'collaborate' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   fetch             Download objects and refs from another repository
'fetch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   pull              Fetch from and integrate with another repository or a local branch
'pull' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   push              Update remote refs along with associated objects
'push' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>'git help -a' and 'git help -g' list available subcommands and some
''git' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>concept guides. See 'git help <command>' or 'git help <concept>'
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>to read about a specific subcommand or concept.
'to' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>See 'git help git' for an overview of the system.
'See' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git status
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>On branch master
'On' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
'Your' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  (use "git pull" to update your local branch)
'use' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>nothing to commit, working tree cleanC:\Users\18046293>git config
'nothing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git config [<options>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Config file location
'Config' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --global              use global config file
'--global' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --system              use system config file
'--system' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --local               use repository config file
'--local' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --worktree            use per-worktree config file
'--worktree' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -f, --file <file>     use given config file
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --blob <blob-id>      read config from given blob object
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Action
'Action' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get                 get value: name [value-regex]
'--get' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-all             get all values: key [value-regex]
'--get-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-regexp          get values for regexp: name-regex [value-regex]
'--get-regexp' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-urlmatch        get value specific for the URL: section[.var] URL
'--get-urlmatch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --replace-all         replace all matching variables: name value [value_regex]
'--replace-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --add                 add a new variable: name value
'--add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --unset               remove a variable: name [value-regex]
'--unset' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --unset-all           remove all matches: name [value-regex]
'--unset-all' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --rename-section      rename section: old-name new-name
'--rename-section' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --remove-section      remove a section: name
'--remove-section' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -l, --list            list all
'-l' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -e, --edit            open an editor
'-e' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-color           find the color configured: slot [default]
'--get-color' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --get-colorbool       find the color setting: slot [stdout-is-tty]
'--get-colorbool' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Type
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -t, --type <>         value is given this type
> was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --bool                value is "true" or "false"
'--bool' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --int                 value is decimal number
'--int' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --bool-or-int         value is --bool or --int
'--bool-or-int' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --path                value is a path (file or directory name)
'--path' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --expiry-date         value is an expiry date
'--expiry-date' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Other
'Other' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    -z, --null            terminate values with NUL byte
'-z' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --name-only           show variable names only
'--name-only' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --includes            respect include directives on lookup
'--includes' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --show-origin         show origin of config (file, standard input, blob, command line)
'--show-origin' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --show-scope          show scope of config (worktree, local, global, system, command)
'--show-scope' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    --default <value>     with --get, use default value when missing entry
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git config --global user.name "David Schoeman"
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git config --global user.email david@rurunz.co.nz
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>git init
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Initialized empty Git repository in C:/Users/18046293/.git/
'Initialized' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293>cd C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git
'C:\Users\18046293' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -am "My first try with Git repository"
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>[master 8603b4a] My first try with Git repository
'[master' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 6 files changed, 4 insertions(+), 1 deletion(-)
'6' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> create mode 100644 .DS_Store
'create' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 HelloWorldInCpp.cpp

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 README.txt

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 Simplecalculator.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 leapYear.java

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> mode change 100755 => 100644 leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'Branch-test'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.java
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add .java
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: pathspec '.java' did not match any files
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'SecondBranch'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.txt
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add *.cpp
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already up to date.
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already up to date.
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:22:11 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:15:55 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    first commit
'first' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: did you mean `--all` (with two dashes)?
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show -branch -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: switch `l' expects a numerical value
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (HEAD -> SecondBranch, master, d-SecondBranch, d-Branch-test, d-, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/.DS_Store b/.DS_Store
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new file mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 0000000..5008ddf
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Binary files /dev/null and b/.DS_Store differ
'Binary' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/HelloWorldInCpp.cpp b/HelloWorldInCpp.cpp
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/README.txt b/README.txt
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/Simplecalculator.py b/Simplecalculator.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.java b/leapYear.java
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.py b/leapYear.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>old mode 100755
'old' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>new mode 100644
'new' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 83a3b28..62117ae
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>--- a/leapYear.py
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+++ b/leapYear.py
'+++' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>@@ -4,10 +4,13 @@
'-4' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> year = int(input("Enter a year: "))
'year' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> if (year % 4) == 0:
% was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    if (year % 100) == 0:
% was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>-       if (year % 400) == 0:           print("{0} is a leap year".format(year))
'-' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+       if (year % 400) == 0:^M
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+           print("{0} is a leap year".format(year))^M
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>            print("{0} is not a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        print("{0} is a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    print("{0} is not a leap year".format(year))
Unable to initialize device PRN

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+^M
'+M' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+print("done")^M
'+print' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>These are common Git commands used in various situations:
'These' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>start a working area (see also: git help tutorial)
The system cannot find the file a.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   clone             Clone a repository into a new directory
'clone' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   init              Create an empty Git repository or reinitialize an existing one
'init' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>work on the current change (see also: git help everyday)
'work' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   add               Add file contents to the index
'add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   mv                Move or rename a file, a directory, or a symlink
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   restore           Restore working tree files
'restore' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rm                Remove files from the working tree and from the index
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   sparse-checkout   Initialize and modify the sparse-checkout
'sparse-checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>examine the history and state (see also: git help revisions)
'examine' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   bisect            Use binary search to find the commit that introduced a bug
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   diff              Show changes between commits, commit and working tree, etc
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   grep              Print lines matching a pattern
'grep' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   log               Show commit logs
'log' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   show              Show various types of objects
'show' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   status            Show the working tree status
'status' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>grow, mark and tweak your common history
'grow' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   branch            List, create, or delete branches
'branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   commit            Record changes to the repository
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   merge             Join two or more development histories together
'merge' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rebase            Reapply commits on top of another base tip
'rebase' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   reset             Reset current HEAD to the specified state
Invalid parameter(s)
RESET { SESSION }

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   switch            Switch branches
'switch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   tag               Create, list, delete or verify a tag object signed with GPG
'tag' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>collaborate (see also: git help workflows)
'collaborate' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   fetch             Download objects and refs from another repository
'fetch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   pull              Fetch from and integrate with another repository or a local branch
'pull' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   push              Update remote refs along with associated objects
'push' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>'git help -a' and 'git help -g' list available subcommands and some
''git' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>concept guides. See 'git help <command>' or 'git help <concept>'
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>to read about a specific subcommand or concept.
'to' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>See 'git help git' for an overview of the system.
'See' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  Branch-test
'Branch-test' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* SecondBranch
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-
'd-' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-Branch-test
'd-Branch-test' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  d-SecondBranch
'd-SecondBranch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  master
'master' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'master' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-Branch-test' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch d- d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: A branch named 'd-' already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-Branch-test
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d-Branch-test (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d- (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch -d d-SecondBranch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted branch d-SecondBranch (was 8603b4a).
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>! [Branch-test] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> ! [SecondBranch] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  * [master] My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>---
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>++* [Branch-test] My first try with Git repository
'++*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git show-branch --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>! [Branch-test] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> ! [SecondBranch] My first try with Git repository
'!' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  * [master] My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>---
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>++* [Branch-test] My first try with Git repository
'++*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git check-out master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: 'check-out' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar command is
'The' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        checkout
'checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Already on 'master'
'Already' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git ls-tree -r master --name-only
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>.DS_Store

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>HelloWorldInCpp.cpp

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>README.txt

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Simplecalculator.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>leapYear.java


C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>leapYear.py

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git branch feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'feature-2'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>M       leapYear.py
'M' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git diff leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>diff --git a/leapYear.py b/leapYear.py
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>index 62117ae..466671e 100644
'index' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>--- a/leapYear.py
'---' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+++ b/leapYear.py
'+++' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>@@ -13,4 +13,4 @@ if (year % 4) == 0:
'-13' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> else:
'else:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    print("{0} is not a leap year".format(year))
Unable to initialize device PRN

 [main 2020-08-03T10:36:27.804Z] update#setState idle

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>-print("done")
'-print' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>+
'+' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git add leapYear.py
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git commit -m "changed leapYear.py"
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>[feature-2 d244b0d] changed leapYear.py
'[feature-2' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 1 file changed, 1 insertion(+), 1 deletion(-)
'1' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: No remote for the current branch.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'feature-2'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: No remote for the current branch.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git checkout master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Switched to branch 'master'
'Switched' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git merge feature-2
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Updating 8603b4a..d244b0d
'Updating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Fast-forward
'Fast-forward' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> leapYear.py | 2 +-
'2' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> 1 file changed, 1 insertion(+), 1 deletion(-)
'1' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log --all --oneline --graph --decorate
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* d244b0d (HEAD -> master, feature-2) changed leapYear.py
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 8603b4a (SecondBranch, Branch-test) My first try with Git repository
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 68892c4 changed
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>* 5b1a3fe first commit
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>(node:9852) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:9852) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: '/help' is not a valid tag name.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag /?
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: '/?' is not a valid tag name.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git /?
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: '/?' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar commands are
'The' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        am
'am' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        gc
'gc' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        mv
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        p4
'p4' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        rm
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -d help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Deleted tag 'help' (was d244b0d)
'Deleted' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>unknown option: -a
'unknown' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git tag -a -m "This is my first annotate tag for the changes to the leapYear file" leapYear
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://github.com/18046293/159251-tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Enumerating objects: 17, done.
'Enumerating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Counting objects: 100% (17/17), done.
'Counting' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Delta compression using up to 2 threads
'Delta' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Compressing objects: 100% (17/17), done.
'Compressing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Writing objects: 100% (17/17), 2.14 KiB | 548.00 KiB/s, done.
'Writing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 17 (delta 6), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>remote: Resolving deltas: 100% (6/6), done.
'remote:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      master -> master
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      Branch-test -> Branch-test
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      SecondBranch -> SecondBranch
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new branch]      feature-2 -> feature-2
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push origin --tags
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Enumerating objects: 1, done.
'Enumerating' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Counting objects: 100% (1/1), done.
'Counting' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Writing objects: 100% (1/1), 203 bytes | 203.00 KiB/s, done.
'Writing' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
'Total' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>To https://github.com/18046293/159251-tutorial1.git
'To' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git> * [new tag]         leapYear -> leapYear
'*' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin master
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin -all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>error: did you mean `--all` (with two dashes)?
'error:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial01.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git remote add origin https://18046293@bitbucket.org/18046293/tutorial1.git
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>fatal: remote origin already exists.
'fatal:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git push -u origin --all
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Everything up-to-date
'Everything' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'Branch-test' set up to track remote branch 'Branch-test' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'SecondBranch' set up to track remote branch 'SecondBranch' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'feature-2' set up to track remote branch 'feature-2' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Branch 'master' set up to track remote branch 'master' from 'origin'.
'Branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git log
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit d244b0d2580f66cfc635914311d727a2ea1d31b5 (HEAD -> master, tag: leapYear, origin/feature-2, feature-2)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:27:42 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed leapYear.py
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 8603b4a2f7741755e146620770dc8adf89792feb (origin/SecondBranch, origin/Branch-test, SecondBranch, Branch-test)
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: David Schoeman <david@rurunz.co.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Aug 3 21:04:57 2020 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    My first try with Git repository
'My' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 68892c479b7f98f76b85a2c38d6b06d35c7ff213
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:22:11 2019 +1200
(node:9852) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:9852) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    changed
'changed' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>commit 5b1a3fe0e152a4de6a1af2a7e67786b45def7acf
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Author: Amjed Tahir <A.Tahir@massey.ac.nz>
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Date:   Mon Jul 22 09:15:55 2019 +1200
The system cannot accept the date entered.
Enter the new date: (dd-mm-yy)

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>    first commit
'first' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git hist
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git: 'hist' is not a git command. See 'git --help'.
'git:' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>The most similar command is
'The' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>        bisect
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git --help
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
< was unexpected at this time.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
'[-p' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
(node:920) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
(node:920) Electron: Loading non context-aware native modules in the renderer process is deprecated and will stop working at some point in the future, please see https://github.com/electron/electron/issues/18397 for more information
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>           <command> [<args>]
The syntax of the command is incorrect.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>These are common Git commands used in various situations:
'These' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>start a working area (see also: git help tutorial)
The system cannot find the file a.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   clone             Clone a repository into a new directory
'clone' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   init              Create an empty Git repository or reinitialize an existing one
'init' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>work on the current change (see also: git help everyday)
'work' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   add               Add file contents to the index
'add' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   mv                Move or rename a file, a directory, or a symlink
'mv' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   restore           Restore working tree files
'restore' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rm                Remove files from the working tree and from the index
'rm' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   sparse-checkout   Initialize and modify the sparse-checkout
'sparse-checkout' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>examine the history and state (see also: git help revisions)
'examine' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   bisect            Use binary search to find the commit that introduced a bug
'bisect' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   diff              Show changes between commits, commit and working tree, etc
'diff' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   grep              Print lines matching a pattern
'grep' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   log               Show commit logs
'log' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   show              Show various types of objects
'show' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   status            Show the working tree status
'status' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>grow, mark and tweak your common history
'grow' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   branch            List, create, or delete branches
'branch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   commit            Record changes to the repository
'commit' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   merge             Join two or more development histories together
'merge' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   rebase            Reapply commits on top of another base tip
'rebase' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   reset             Reset current HEAD to the specified state
Invalid parameter(s)
RESET { SESSION }

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   switch            Switch branches
'switch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   tag               Create, list, delete or verify a tag object signed with GPG
'tag' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>collaborate (see also: git help workflows)
'collaborate' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   fetch             Download objects and refs from another repository
'fetch' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   pull              Fetch from and integrate with another repository or a local branch
'pull' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>   push              Update remote refs along with associated objects
'push' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>'git help -a' and 'git help -g' list available subcommands and some
''git' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>concept guides. See 'git help <command>' or 'git help <concept>'
The system cannot find the file specified.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>to read about a specific subcommand or concept.
'to' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>See 'git help git' for an overview of the system.
'See' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>git status
'C:\Users\18046293\Downloads\Tutorial' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>On branch master
'On' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
'Your' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>  (use "git pull" to update your local branch)
'use' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>
C:\Users\18046293\Downloads\Tutorial 1- Git\Tutorial 1- Git>nothing to commit, working tree clean










