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

#### Change repository name
[Lindsey - add pick of where to go in github to change a repo name]


#### `.gitignore`
- touch .gitignore
- go to link of python gitignore file and copy content
- vim .gitignore
- i
- paste file content
- add `.DS_Store/` and  `.ipynb_checkpoints` to gitignore
- esc
- :wq
- git add/commit/push

#### Remove unnecessary files
Why you need to use a `git rm` vs `rm` or `delete`
- `git rem filename`

#### Images folder
- `mkdir images`
- git add/commit/push

#### Move image files
- `git mv`

#### Update file names
- also `git mv` !


To recap, we used the following code for these changes:
[image of whole  code terminal]


[Lindsey add post pics for each update]

Clone the messy repo to your local machine and see if you can replicate these changes using github and the terminal

