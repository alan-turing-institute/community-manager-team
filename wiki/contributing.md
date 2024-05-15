---
title: "Contributing"
---

## How is the Wiki built?

The RCM Wiki is built with [Quarto](https://quarto.org), an open-source scientific and technical publishing system. ==**By using quarto on git(hub)**== we are developing and modeling best practice in recording and communicating research in data science. We practice in this way so that we may support our communities in doing the same :).

We invite you to contribute to develop your own skill and practices with these tools.

## Where to start

==**Prerequisits, e.g. git, github accounts. Link to resources**==

<!-- Unlike Jupyter Book or RMarkdown, it isn't a package that belongs to a programming language, it's a javascript based Command Line Interface (cli) program that supports embedding multple languages within Quarto documents.  -->

The Wiki is deployed via GitHub Pages on the `gh-pages` branch. This means if you want create a Pull Request to edit the wiki, you will want to merge any branches with `gh-pages` rather than `main`.


## Do I need to download any software to contribute?

At the moment - yes. You need a local install of Quarto to render `.qmd` files.
Some IDEs already come included with Quarto:

1. VSCode + [VSCode Quarto Extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto)
2. RStudio (comes with Quarto)

Or you could download the [Quarto CLI](https://quarto.org/docs/download/) if you like working on a terminal. 

#### Can I just edit directly on GitHub?
Soon! We are working on integrating the Quarto GitHub Action and Deploy Preview to allow rendering and deployment entirely from with the GitHub repository.

## How do I work with Quarto to edit the Wiki?
Working with Quarto is largely working with markdown files. 
Where GitHub and HackMD use vanilla `.md` markdown files to write README files, Quarto has it's own flavour of markdown file called a `.qmd` file.
If you have ever edited a markdown file before, you will be at home with writing markdown files in Quarto - and this is *mostly* all you need to build this wiki.

### The `_quarto.yml` file
The other important file for this Wiki, and for Quarto in general is the `_quarto.yml` file. 
The reason you see links on the navigation bar, or sections on the left sidebar is because they are specified to look that way in the `_quarto.yml`.

### File structure of the website
The `index.qmd` at the base of the repository serves the homepage. Any other sections on the website exist as a subdirectory of `_site/`. For example, the page you are viewing now is built from `_site/contributing/index.qmd`. In the `quarto.yml` file there will be a reference to this file path in the section that defines the top navigation pane.

## I'm getting the hang of Quarto - what next?
Once you are comfortable editing `.qmd` files and slotting them into the `_quarto.yml` file, you can *change the way this wiki looks* by:

1. Cloning the repository to your local desktop
2. Create an switch to the new branch with `git checkout -b mynewbranch`
3. Edit or create `.qmd` file(s)
4. Make changes to the `_quarto.yml` file (if needed)
5. Render the website (and show a preview):
    - **In VSCode**:
        Use the Quarto Extension and press "Render" when you have any `.qmd` file open
    - **In RStudio**:
        Press "Render" when you have any `.qmd` file open
    - **On the Command Line**:
        At the top of the local cloned directory you can run `quarto preview index.qmd` and this will provide you with a `localhost` URL that you can visit and check your changes.
6. Push the change to GitHub `git push --set-upstream origin mynewbranch`
7. In the Pull Request ensure that you are merging to the `gh-pages` branch, not the `main` branch.

## Practice here!
This is an open space to pracice editing this repository :). Feel free to add your name, or favourite pizza topping in the space below and submit a Pull Request! 

* Cass thinks pinenuts make pizza a bit posh! 




::: callout-note
##
You can also click on "Edit this page" on the right hand side of this page. This takes you directly to the page on the GitLab website and you can edit directly - don't forget to create a new branch at the bottom of the page on GitLab when you commit these changes!
:::

