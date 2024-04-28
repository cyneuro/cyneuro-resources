# CyNeuro Resources

Useful links:
- [jupyter-book](https://jupyterbook.org/en/stable/intro.html) official documentation, provides detailed instructions on how to add, edit, and publish content.
- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), a guide to editing markdown files. 
- [PyData theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/user_guide/index.html) official documentation, provides instructions on advanced UI settings. 
- [fontawesome](https://fontawesome.com), a collection of icons used on the web (useful for navigation bar links).
 - [decodeunicode](https://decodeunicode.org/en), number codes for free unicode symbols and emojis. 
    

## Requirements

```bash
pip install jupyter-book
pip install pydata-sphinx-theme
pip install ghp-import
```

We can use `jupyter-book` to build the pages from source and `ghp-import` to publish them. We are using the PyData theme which is installed by `pydata-sphinx-theme`.

## Adding / Editing Pages

1. Create a file and save it somewhere in the repository (or edit an exsisting file).
2. Add the path to the file to `_toc.yml` ([rules](https://jupyterbook.org/en/stable/structure/toc.html)). If the path is already in the `_toc.yml`, skip this step.
3. Go to the directory containing the `cyneuro-resources` repo. Rebuild the pages with
```bash
jupyter-book build cyneuro-resources
```
It might throw warnings, but if you see the "Finished generating HTML for book" message between two green lines, then the build was successful. The message will also contain HTML address which you can use to view the resulting build locally. To do that, copy them from the terminal to a browser. 
4. If the local build is fine, add, commit and push the changes to the source files.
```bash
cd cyneuro-resources
git add .
git commit -m 'type a message'
git push
```
5. Publish the compiled HTML files with
``` bash
ghp-import -n -p -f _build/html
```