# The Oberlin Motion Lab Web Site

## How do I use this repository?
### First, clone the repo into your desired workspace.
##### For macOS:
First, click on the green button that says "Clone or Download" on the top right of this repository. Then click the small grey clipboard icon next to the link. Don't copy anything else until we use that link in a moment.

Open your [terminal](http://blog.teamtreehouse.com/introduction-to-the-mac-os-x-command-line).

Go to your desired parent directory:
```
cd ~\pathTo\myDirectory
```
Then create the directory you want to copy this repository into. For instance:
```
mkdir OMLSite
```
Now go into that directory
```
cd OMLSite
```
And clone the repository
```
git clone --recursive (paste copied repository link here without parentheses)
```
You might be wondering what each of these commands mean. Well
```
git
```
Allows you to interface with the [git version control system](https://guides.github.com/introduction/flow/).
```
clone
``` 
is a git command to copy a repo's codebase onto your computer, and 
```
--recursive
```
is a special flag for the clone command that says you want to not only copy this repository's codebase, but also the code from the repositories that this repo links to.

If that doesn't make sense, then look at the folders in our code at the top of this page, you'll see
- content/
- public @ ed66245/
- static/
- themes/

Now click on the public folder.

See how the whole repository changed? It brought you to our other repository that we use to house the published content for the site. 

That public directory is called a submodule, and if you don't use the `--recursive` flag you won't get the code from that repository when you clone this one. 
