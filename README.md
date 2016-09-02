Command Line Use:

```
pandoc [input] -o [output].pdf --latex-engine=lualatex --latex-engine-opt=-shell-escape -fmarkdown-implicit_figures
```


pandoc vespers.md -o vesper-draft-2016-09-01.pdf --latex-engine=lualatex --latex-engine-opt=-shell-escape -fmarkdown-implicit_figures




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
