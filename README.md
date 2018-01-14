## My Git Workspace

My Git Workspace has a custom prompt. My name is in purple and the directory
name is in blue.  If I change directory (cd) to a Git repository, the prompt
shows in green which commit I have currently checked out.

This configuration is also cool the visualize the edition workflow. If I change
something without commiting, the prompt will show a star, for instance, (master
\*). Moreover, it has tab completion set up for git commands.

In order to have my Workspace follow the instructions bellow (the three files
mentioned are available at https://github.com/pdelfino/git-udacity):

+ Save git-completion.bash file in your home directory with the name
git-completion.bash.

+ Save git-prompt.sh in your home directory with the name git-prompt.sh.

+ Download bash\_profile\_course.

I am using Linux/Ubuntu, so I needed to to name this file .bashrc instead of
.bash\_profile.

Now, run the following commands (vim is my favorite text editor, you may need
to adapt the first command):

```bash 
git config --global core.editor "vim" 
git config --global push.default
upstream git config --global merge.conflictstyle diff3

```

