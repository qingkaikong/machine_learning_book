# Book format

The book is written in Jupyter notebook, texts are in the markdown cells, and codes are in the code cells.

# Naming of the notebooks

Let's have consistent naming for all the notebooks. 

The notebook name should follow the following format

```
 ChapterXX.YY-Name-of-The-Chapter.ipynb
```
Where XX start with 01, and YY start with 01. 

# About the Auto-Numbering

To reduce the efforts keeping tracking all the numbers showing each chapter and sub-section. I use the auto-numbering function that is defined in the *_toc.yml*. But it has some constraints:

* The notebook that in the chapter section, if you add any sections there, it will automatically add into the 2nd level, therefore, don't add any sections in this file. 

* The subsection files should start with # (this will be the 2nd level numbering, such as 1.1, 1.2 etc). Then adding any sections here will add next level, such as ## will be 1.1.1.

* In *_toc.yml*, I only allow 3 levels numbering, therefore, anything further than ### will not be numbered.  

# Inside of the notebooks

The following comes from [Jupyter book recommendations](https://jupyterbook.org/file-types/index.html#rules-for-all-content-types). 

* Files must have a title. Generally this means that they must begin with a line that starts with a single #

* Use only one top-level header. Because each page must have a clear title, it must also only have one top-level header. You cannot have multiple headers with single # tag in them.

* Headers should increase linearly. If you’re inside of a section with one #, then the next nested section should start with ##. Avoid jumping straight from # to ###.
