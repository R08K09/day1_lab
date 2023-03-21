## Terminal cheatsheet for reference

### Terminal Commands

* `pwd` - prints the name of the working directory
* `cd` - change directory
  * `cd ..` - moves back up to the previous directory
  * `cd (name)` - moves down into (name) folder
  >  * . (Single Period) - Current directory
  >  * .. (Double Period) - Parent directory
  >  * ~ (Tilde) - Home directory
* `mkdir` - creates a directory within current directory
  * For example:
    * mkdir bnta_work
    * mkdir bnta_work/week_01
    * mkdir bnta_work/week_01/day_1
* `touch` - create new empty files
* `mv` - move files
* `rm` - removes folder/file completely (be cautious!)
  * `rmdir` - removes directory but only if empty
  * `rm -r` deletes a directory and all of its child directories
* `ls` - lists folders and files inside the current directory
  * `ls -a` - does the same as `ls` but includes hidden files and directories
  * `ls -t` orders files and directories by the time they were last modified.
* `open` - opens the current folder or file in finder
* `q` - quit sub-screen and return to terminal
* `clear` - clear terminal screen of all previous commands, so it's blank


### Git Commands/Steps Example

* `git status` - displays the state of the working directory and the staging area
* `git init` - creates a new Git repository
* `git add (file)` - adds a change in the working directory to the staging area so updates are included in the next commit 
* `git commit -m"(some message)"` - captures a snapshot of the project's currently staged changes
* `git log` - displays snapshots of the project's committed history
* `git push` - sends the committed changes to remote repositories

#### Create the git repository and file

1. Enter directory you want to create a repository in
2. Type `git init` to initialise empty Git repository in current directory
   * can check if git has been initialised by typing `ls -a` and a `.git` should appear
3. Create an empty file e.g. `touch (file)`
   * can check if file was made by typing `ls` and the file should appear
4. Recommend to use `git status` to continuously check
5. Type `git add (file)` to add untracked file facts.txt, so it's ready to be committed
6. Repeat step 4 to check status
7. Type `git commit -m"adds (file)"` to commit tracked file
   * All commits have to be accompanied by a message (typically in present tense)
8. Type `git log` to check the history of git, press `q` to exit
9. `git status` will not show that nothing needs to be committed

#### Currently, facts.txt is an empty file so let's add something inside the file.

1. Still in git, type `open .` to open our directory in finder
2. Open our `file` in TextEdit and modify it by adding a sentence
3. If we check `git status`, we will be informed that the file has been modified but change has not been committed
4. Same as before, `git add .` to add all changes to git
5. Status shows that it's now ready to be committed
6. Type git commit -m"adds penguin fact"
7. `git log` will show us the updated history of this git

#### Create the repository in gitHub.com (steps explained below)

1. In account home, in top right corner, select the plus symbol and select new repository
2. Type in repository name - typically same name as directory
3. Keep it public so others can see it
4. Then click on Create Repository
5. Make sure that SSH is selected and not HTTPS
6. Copy the code block for pushing an existing repository from the command line

#### Push the file to gitHub

1. Paste the code block into the terminal and run it
2. File should now be seen on gitHub under the repository name

#### If we make another change that requires another commit

1. Again, use `git add` and `git commit -m"(some message)"` to commit the change
2. Except now, type `git push` as we do not need to paste the code block again



#### Handy Terminal shortcuts to save time

> 1. Use tab key to autocomplete names rather than typing out the whole thing
>    * Start typing cd (name initial) and press the tab key. 
>    * A list of possible docs/folders should appear, then select the correct one
>
> 2. Use the up and down keys to show previous commands in the terminal. It can save some time.



#### Markdown style tips

The amount of (#) affect the heading size, the less #'s the bigger the text size.

For **bold** __text__, use ** or __ on either side of the word or phrase.

For *italicize* _text_, use just 1 * or _ on either side of the word or phrase.

To do both ***bold*** and ___italics___, use three * or _ in any combination on either side of the word or phrase,
e.g. *** or ___ or (__*) or (**_)

> Note: This will appear differently
>> And this is a nested blockquote

We can have ordered and unordered lists
1. One
2. Two
3. Three

* A
* B
* C
  + and this one is indented

If you want to emphazise something, you can use `backticks` 

