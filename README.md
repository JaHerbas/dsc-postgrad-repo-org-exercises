# Repository Update Code Along

## Learning goals
- list the steps taken to clean the messy repository example
- reproduce those steps locally on your own machine

To align the messy repo with industry expectations you will:

- Use Github to change the name of the directory to something meaningful
- Use git through terminal to:
  - Create a `gitignore` file in terminal
  - Remove unnecessary files
  - Create a folder for images
  - Move image files to the new folder
  - Rename indiviudal files to more  descriptive names

#### Fork and Clone
To follow along with these steps and replicate locally, first fork [this repository] and clone to your local machine.

#### Change repository name
A repository name should be informative about its contents. Which repository name tells more to employers?

- example one
- example two
[Lindsey, update the above]

There are two ways to change the name of a github repository. It [can be done through the terminal and through github online.](https://help.github.com/en/github/administering-a-repository/renaming-a-repository).

This example shows using the github repository website. 

[Lindsey - add pic like in the link above, but with our updated directory name]


#### `gitignore`
The [`gitignore`](https://git-scm.com/docs/gitignore) file tells git which files to "ignore" and not track. Each line in a `gitignore` list the string pattern in your directories that git should not track. Many hidden system files, caches, and output directories do not need to be tracked for a project or would cause problems on another person's system if they were to clone and pull your system files to their computer. 

Github provides [many sample `gitignore` templates](https://github.com/github/gitignore) based on the languages or tools of your project. The [python `gitignore`](https://github.com/github/gitignore/blob/master/Python.gitignore) is the best choice for most Flatiron School data science projects. If a specific file or directory type is not listed in a `gitignore` template it is not a problem. `gitignore` files can be updated through vim in terminal or edited on github. The steps below walk through creating a `gitignore` file from scratch, using the python `gitignore` template, and adding specifications to the file. 

**Create `gitignore` file**
- touch .gitignore

**Get template**
- go to [link of python gitignore](https://github.com/github/gitignore/blob/master/Python.gitignore) file and copy content

**Add content to `gitignore`**
- vim .gitignore
- i
- paste file content

**Tell git to ignore more files**
- add `.DS_Store/` and  `.ipynb_checkpoints` to gitignore
- esc
- :wq

**Save changes**
- git add/commit/push

#### Remove unnecessary files
While tracking data transformation and cleaning before modeling is important, Github is not the place to store those datasets. [Github has a firm limit on file size](https://help.github.com/en/github/managing-large-files/conditions-for-large-files) and it [takes extra work to remove large files](https://help.github.com/en/github/managing-large-files/removing-files-from-a-repositorys-history) from a repository if you commit them by mistake. It is best to either store your data locally and add `csv`, `json`, and such file types to your `.gitignore` file.

For this exercise, you will follow how the datafile is removed using [`git rm`](https://git-scm.com/docs/git-rm). `git rm` will remove a file both from the local directory **and** from your repository when you push. If you only use a `delete` or ` rm` locally without using `git rm`, the file will still be stored remotely and be downloaded again with future `pull` commands.

- `git rm filename`
- git add/commit/push

#### Images folder
The top level of the repository directory needs to uncluttered and direct employers to what they need to see. All files are on the same level in the messy repository example. The image files, while important to our notebook, are merely clutter to a future employer. Creating subdirectories to store non-priority files will solve this problem. Use `mkdir` to create a new folder within your directory. But **note**, the folder will not show up in the remote repository until files are **in** the folder.

- `mkdir images`


#### Move image files
[`git mv`](https://git-scm.com/docs/git-mv) is another command that both physically moves a file **and** updates the index within the git file in one step. The syntax of the `git mv` is:

`git mv oldlocation\filename  newlocation\filename`

So in this example, the following code will move the image files to the newly created directory:
[Lindsey work here]
- `git mv`

#### Update file names

The file names should also be informative. `git mv` can also be used to rename files!

[lindsy example stuff]
- also `git mv` !


To recap, we used the following code for these changes:
[image of whole  code terminal]


[Lindsey add post pics for each update]

Clone the messy repo to your local machine and see if you can replicate these changes using github and the terminal

