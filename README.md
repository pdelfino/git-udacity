# Git and GitHub -- Udacity Course

![The Ancient of Days](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ac/Europe_a_Prophecy_copy_K_plate_01.jpg/960px-Europe_a_Prophecy_copy_K_plate_01.jpg)

*"The Ancient of Days" (1794) by William Blake — [Wikipedia](https://en.wikipedia.org/wiki/The_Ancient_of_Days)*

Custom Git workspace configuration and learning reflections from Udacity's *How to Use Git and GitHub* course.

## About

Materials from [How to Use Git and GitHub](https://br.udacity.com/course/how-to-use-git-and-github--ud775) on Udacity. This repo includes a polished Git workspace setup with a custom prompt, tab completion, and dirty-state indicators, along with reflections written during the course.

## Custom Git Workspace

![Custom Git prompt](https://media.giphy.com/media/wKcfPVI7QXUaqQzgfp/giphy.gif)

**Features:**

- Username displayed in purple
- Current directory in blue
- Git branch name in the prompt
- Tab completion for Git commands
- Dirty-state indicators:
  - `*` -- unstaged changes
  - `+` -- staged but uncommitted changes

## Setup Instructions

1. Save `git-completion.bash` in your home directory.
2. Save `git-prompt.sh` in your home directory.
3. Add the following to your `.bashrc`:

```bash
# Enable tab completion
source ~/git-completion.bash

# Colors
green="\[\033[0;32m\]"
blue="\[\033[0;34m\]"
purple="\[\033[0;35m\]"
reset="\[\033[0m\]"

# Custom prompt with Git integration
source ~/git-prompt.sh
export GIT_PS1_SHOWDIRTYSTATE=1
export PS1="$purple\u$green\$(__git_ps1)$blue \W $ $reset"
```

4. Configure Git defaults:

```bash
git config --global core.editor "emacs"   # or your preferred editor
git config --global push.default upstream
git config --global merge.conflictstyle diff3
```

## Course Reflections

Written reflections on version control concepts, completed as part of the course exercises:

- [Lesson 1](https://github.com/pdelfino/git-udacity/blob/master/lesson_1_reflection_prompts.txt) -- diffs, commit history, file versioning
- [Lesson 2](https://github.com/pdelfino/git-udacity/blob/master/lesson_2_reflection_prompts.txt) -- branching and merging
- [Lesson 3](https://github.com/pdelfino/git-udacity/blob/master/lesson_3_reflection_prompts.txt) -- collaboration with GitHub

## Tech Stack

- **Shell:** Bash
- **Tools:** Git, GitHub

## Notes

- Reflections are written in Portuguese.
