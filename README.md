
# Faden LaTeX package
This latex style file was created for my own personal use. 

It is inspired by [Kieran Healy](http://kieranhealy.org/).

Besides looking great, the `.sty` file also loads a bunch of packages, custom math commands, and theorem environments.

![Example](https://www.dropbox.com/s/vt6s6ow3e4vu9hc/latexpackage1.png?dl=1 "Example")

## Packages

- fixltx2e  

#### Math

- mathtools                 
- amsthm                    
- bm     

#### Figures and tables

- booktabs                  
- subcaption                
- pgfplots
- tikz 

#### References

- hyperref                  
- cleveref     

#### bibliography

- csquotes
- biblatex

#### Misc.

- todonotes           
- url                       
- appendix              
- accents 
- xparse

#### Index

- imakeidx                
- xstring
- xcolor

#### Version control
 - Version control with the VC package. See [The VC package](https://www.ctan.org/tex-archive/support/vc?lang=en) on CTAN

## Thorems

```latex
% Theorem Styles
\newtheorem{theorem}{Theorem}[section]
\newtheorem{lemma}[theorem]{Lemma}
\newtheorem{proposition}[theorem]{Proposition}
\newtheorem{corollary}[theorem]{Corollary}
\newtheorem{assumption}[theorem]{Assumption}
% Definition Styles
\theoremstyle{definition}
\newtheorem{definition}{Definition}[section]
\newtheorem{example}{Example}[section]
\theoremstyle{remark}
\newtheorem{remark}{Remark}
```

## Custom Math

```latex
% math
\newcommand{\ubar}[1]{\underaccent{\bar}{#1}} % underbar
\global\long\def\argmax{\operatornamewithlimits{arg\, max}} % argmax

% partial derivative with optional  arguments
\usepackage{xparse} %needed for DeclareDocumentCommand
\DeclareDocumentCommand{\pder}{ O{} O{} m }{\frac{\partial^{#2}#1}{\partial#3^{#2}}}

% Sets
\newcommand{\R}{\mathbb{R}}
\newcommand{\N}{\mathbb{N}}
\newcommand{\Z}{\mathbb{Z}}
```


## Requirements
A working tex system with all of the above package installed