Command Line Use:

```
pandoc [input] -o [output].pdf --latex-engine=lualatex --latex-engine-opt=-shell-escape -fmarkdown-implicit_figures
```


pandoc vesper-shell.md -o vesper-draft-2017-01-26.pdf --latex-engine=lualatex --latex-engine-opt=-shell-escape -fmarkdown-implicit_figures

pandoc 2017-01-26-vespers-insert.md -o 2017-01-26-vespers-insert.pdf --latex-engine=lualatex --latex-engine-opt=-shell-escape -fmarkdown-implicit_figures


At top of `.gabc` file:

```
% !TEX TS-program = LuaLaTeX+se
% !TEX root = main-lualatex.tex
```

At top of `.md` file:

```
---
header-includes:
    - \usepackage[autocompile]{gregoriotex}
---
```

At chant-score insertion:

```
\gregorioscore{cherubic-hymn}
```
# vespers
