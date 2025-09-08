# 2YR

My (Benjamin L Cookman's) second year report for my PhD at UoM.

## LaTeX Compilation

Source code is compiled with:

```bash
mkdir -o out # makeout
lualatex --synctex=1 --interaction=nonstopmode --output-directory=out --output-format=pdf # lualatex
biber --output-directory=out main # biber
lualatex --synctex=1 --interaction=nonstopmode --output-directory=out --output-format=pdf # lualatex
lualatex --synctex=1 --interaction=nonstopmode --output-directory=out --output-format=pdf # lualatex
mv "./out/main.pdf" # movepdf
```

Notice no `git commit` is performed at the end, but may done automatically along with the rest of it using latex tools and recipes in VS Code.

