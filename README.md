My Git Workspace
===

My Git Workspace has a ```custom prompt```. 

+ User name is in purple;

+ The directory name is in blue; and,

+ it has tab completion set up for git commands.

![Alt Text](https://media.giphy.com/media/wKcfPVI7QXUaqQzgfp/giphy.gif)


Visualize the workflow
===

If I change something without adding to the staging area, the prompt will show a ```*```

```pedro (master *)```

If I change something without comitting, the prompt will show a ```+```


```pedro (master +)```

Mimic me
===

In order to have my Workspace follow the instructions bellow (the three files
mentioned are available [here](https://github.com/pdelfino/git-udacity)):

+ Save ```git-completion.bash``` file in your home directory with the name
```git-completion.bash```;

+ Save ```git-prompt.sh``` in your home directory with the name 
```git-prompt.sh```;  and,

+ Download ```bash\_profile\_course```.

I am using ```Linux/Ubuntu```, so I needed to to name this file ```.bashrc``` 
instead of ```bash_profile```.

Now, run the following commands (vim is my favorite text editor, you may need
to adapt the first command):

```bash 
git config --global core.editor "vim" 
git config --global push.default
upstream git config --global merge.conflictstyle diff3
```


Reflections
=== 

During the course  ["How to use Git and Github"](https://br.udacity.com/course/how-to-use-git-and-github--ud775) on Udacity,
professors encouraged us to write reflections about the classes.

Here you can check out three files with my reflections and some shortcuts for git. Sorry for the draft style:

+ [first](https://github.com/pdelfino/git-udacity/blob/master/lesson_1_reflection_prompts.txt)

+ [second](https://github.com/pdelfino/git-udacity/blob/master/lesson_2_reflection_prompts.txt)

+ [third](https://github.com/pdelfino/git-udacity/blob/master/lesson_3_reflection_prompts.txt)
