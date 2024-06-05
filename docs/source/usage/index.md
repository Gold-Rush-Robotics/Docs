
# Quick Links and Notes

## Quick Links to docs
[Markdown Plugin](https://myst-parser.readthedocs.io/en/latest/index.html) <- look here for translating sphinx commands into markdown

[Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) <- look here to customize how something looks

## Setting up your enviroment

clone the code
```bash
git clone https://github.com/Gold-Rush-Robotics/Docs.git
```

cd into the repo
```bash
cd Docs/
```

make a virtual env
```bash
python3.8 -m venv venv
source venv/bin/activate
pip install -r docs/requirments.txt
```

build the docs locally
```bash
cd docs/
make html
```

Then you can find the docs in _build/html/index.html

Once you are satisfied with your changes push them up!


## Quick tips and tricks

The docs will try to auto build and deploy when you push to main (yay CI/CD)

### Creating new files

Each new file needs a title which you can make with # and then a space then some text

(Feel free to click view source to see how this one is working)

````{tip}
Make sure to include any new file you make in a toctree directive higher up or it won't show up anywhere


    ```{toctree}
    relative/file/path
    ```
````

### Markdown syntax quick ref

#### Headers
use # for headers the number of # is the header level so # is H1 and ## is H2

#### Emphasis
- use \* for *italics*
- use \** for **bold**
- use \~~ for ~~strikethrough~~

#### Lists 
- Unordered list with \-
    * Or with \*
1. Ordered lists are just \1.

- [ ] If you want to be fancy \- [ ]
- [X] You can make task lists \- [X]

#### Random stuff 

H{sub}`2`O subscripts with {sub}\`2\`

coming soon{sup}`tm` or superscripts {sup}\`tm\`

> oogly boogly quotes with \>


```python
def syntax_highlighting():
    # you can do syntax highlighted code
    print("this is cool....")
    return 0
```

use \```python for syntax highlighting

Dont forget footnotes! [^footnotefun]

[^footnotefun]: This footnotes is hype

for more cool markdown check out the docs 

| Syntax Type  | Quick Link  |
| :----------- | :---------- | 
| Admonitions | [callouts](https://myst-parser.readthedocs.io/en/latest/syntax/admonitions.html) |
| Images and figs | [Whaaat](https://myst-parser.readthedocs.io/en/latest/syntax/images_and_figures.html) |
| Tables | [Like this](https://myst-parser.readthedocs.io/en/latest/syntax/tables.html) |
| Cross Refrences | [👀](https://myst-parser.readthedocs.io/en/latest/syntax/cross-referencing.html) |
| Math and equations | [$a^2 + b^2 = c^2$](https://myst-parser.readthedocs.io/en/latest/syntax/math.html) | 