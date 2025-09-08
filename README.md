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

Notice the `git commit` performed at the end, which is done automatically along with the rest of it using latex tools and recipes in VS Code.


