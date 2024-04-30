### How to install?
- Install LaTeX locally (e.g. [basicTex](https://www.tug.org/mactex/). Missing packages can be installed afterwards using `tlmgr`).

- I use the latex ugent2016 template created by Niko Strijbol. Installation of this template is as easy as going to [this](https://github.com/niknetniko/ugent2016) repo. Downloading the latest release zip (at the time of writing this is 0.10). When unzipping this zip there will be a tds zip available with the name `ugent2016.tds.zip`. To install everything you need to unzip this tds zip at the right place. Right now this is at `/usr/local/texlive/2023basic/texmf-dist` for me. But this directory should contain a `source`, `tex` and `doc` folder among other folders. The `tex` folder should have a subfolder called `latex`. After unzipping the only thing that needs to happen is re-indexing. This can be done by executing `texhash`.

### Generating the PDF
Just run `make` in the `thesis` directory.  
The makefile uses `latexmk` to compile the pdf, this can be installed with using following command
```
tlmgr install latexmk
```
The resulting PDFs can be found back in the `out` directory.