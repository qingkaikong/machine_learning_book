# Book Setup

This book is written in [Jupyter Book](https://jupyterbook.org/intro.html). The setup of the book basically follows [this page](https://jupyterbook.org/start/your-first-book.html).

# Repo Structure
machine_learning_book/  
├── _config.yml - configuration file  
├── _toc.yml - table of content   
├── index.md - the welcome page  
├── requirements.txt - dependencies  
├── logo.png - logo file   
├── references.bib - citation (update later)   
├── notebooks - folder contains notebooks   
├── docs - folder contains documentation   
└── _build - output of jb build  

# Working on the Book

**In master branch**
1. change the source files, i.e. add/modify notebooks or markdown files. The chapter files are in the notebooks folder, but if you want to use markdown files, it is fine too.   
2. update the _toc.yml, which contains the table of content. Only the files specified here will be shown on the website.   
3. git add and push the changed contents to remote master branch   
4. build the book using command ``jupyter-book build --all machine_learning_book``. Note that, the output files will be stored in the _build folder. I've already specify it in the *.gitignore* file.   
5. You publish the book  using the command ``ghp-import -n -p -f _build/html``. Note, *ghp-import* will automatically push the *_build* folder to the gh-pages branch. 

**In gh-pages branch**

This is the branch host the website, I've already set this as the default branch to host website. Therefore, only published stuff should be here (output from the build command in the 5th point above). 