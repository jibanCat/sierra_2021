# UC Sierra Conference 2021 Bio and Poster Templates

Poster templates for UC Sierra Conference 2021. All of them on based on this [overleaf template by LianTze Lim](https://www.overleaf.com/latex/templates/yet-another-beamerposter-theme-with-variable-sizes-and-colour-themes-landscape/tcwvmhjsfbdk), with modifications on the colors from each campus' marketing website. Modifications are made by Ming-Feng Ho (UCR).

- **For personal bio submission, please use the template provided.**
- For research poster submission, feel free to modify the templates here or use any other templates you have.

![](images/all_templates.png)

## How to use them?

### Compile option 1: Overleaf

Overleaf is a cloud-based LaTex editor. It handles the environment for us. The LaTex environment is installed on their server, so no need to install anything.

At this **GitHub repo**, click **Code** -> **Download ZIP**.

Go to https://www.overleaf.com/. Register an account.

Open a **New Project** -> **Upload Project** -> select the `sierra_2021-main.zip` you just downloaded from this repo.

Then you are all set!

Just click the template from your campus and edit it.
When you are done, click **Recompile** to compile everything.

### Compile option 2: Local machine

First clone the repo to your local machine:
```bash
git clone git@github.com:jibanCat/sierra_2021.git
```

> Note: if you prefer https clone, do the following line instead:
> ```bash
> git clone https://github.com/jibanCat/sierra_2021.git
> ```

There are 9 different Tex templates:
`<campus>-template.tex`, campus = ["UCB", "UCD", "UCI", "UCLA", "UCM", "UCR", "UCSB", "UCSC", "UCSD"].
Each Tex template has a color style file: `beamercolortheme<campus>colour.sty`.
And all templates use the same poster style file: `beamerthemeLLT-poster.sty`.

The following we will use UCM as an example.

Suppose we have latex installed on our local machines.
To compile the `.tex` file of UCM:
```bash
pdflatex UCM-template.tex
```

Then we will have the `UCM-template.pdf` generated in the current directory.

> Warning: make sure `beamercolorthemeUCMcolour.sty`, `beamerthemeLLT-poster.sty`, and `images/` are in the current directory.

