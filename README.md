# My LaTeX setup

This repository contains all my setup preferences to work offline with LaTeX.

## Installation

You will first need to install the package `texlive-full` to run LaTeX locally

```bash
$ sudo apt-get install texlive-full
```

Then, install Visual Studio Code Editor

```bash
$ sudo apt install software-properties-common apt-transport-https wget

$ wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

$ sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

$ sudo apt install code
```

Of course, don't forget to update and upgrade

```
$ sudo apt-get update
$ sudo apt-get upgrade
```
After that, install LaTeX Workshop extension by opening the VS Code Quick Open (Ctrl + P), pasting the following command, and pressing enter.

```
ext install James-Yu.latex-workshop
```

Now replace the file `texconfigs/latex.json` of this repository in the folder located at 

```
~/.vscode/extensions/james-yu.latex-workshop-8.19.2/snippets
```

Note that the name of the extension may be different due to versioning. You can also change the file adding/editing the snippets as you wish.

Finally, the file `texconfigs/settings.json` contains not only necessary code for the well-functioning of my setup, but also my whole VS Code preferences. Feel free if you want to only add the LaTeX part.

You will need to replace the file in the folder located at

```
~/.config/Code/User
```


## Usage

+ The folder `bib` contains `.bib` files to use as reference in LaTeX works;
+ The folder `output` contains some useful files for fast compiling, note that you do not need to save the files, when you compile a `.tex`, it will generate then automatically (that's why it is in the `.gitignore`);
+ The folder `pdfs` contains the generated `.pdf` file of all `.tex` files in the main directory;
+ The folder `style` contains my `.sty` preferences, feel free to add yours too;
+ The main directory has a file called `template.tex` which can be used as a template example.
  

## License
[MIT](https://choosealicense.com/licenses/mit/)