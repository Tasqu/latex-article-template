# latex-article-template

A simple LaTeX article template.

This template is intended to be used for preparing drafts of manuscripts for journal submissions,
and contains typical common elements found in final journal templates.
Please note that journals don't always allow publishing of preprints using their templates,
so having a different template during manuscript preparation can make publishing preprints easier.

The template is modularized as much as possible, with the `main.tex` tying it all together.
This is done to facilitate swapping the contents onto a new template for submission,
although sometimes journals require all LaTeX source to be in a single file.
Similarly, I've tried keeping the amount of packages used by the template to a minimum,
as this lessens the probability of conflicts with journal submission templates.


## Use

Just clone or download the template to start working with it in LaTeX locally.
Alternatively, you can fork it and use e.g. Overleaf GitHub integration.

**Remember to delete the `LICENSE` and `README` files when using the template for manuscript preparation!**
You probably don't want your manuscript in the public domain 😉


### Revisions and review

Collaborating with LaTeX through Git is not the best, but doable.
For example if working in GitHub, revisions should likely be handled through separate branches and pull requests per reviewer.

The template also contains a suggested format for review comment highlights, which can be ignored/removed if desired.
Example commands `\reva{text}` and `\revb{text}` for reviewers A and B, respectively, are defined in `main.tex` for highlighting reviewer comments/changes:
```latex
\usepackage{xcolor} % Required for coloured highlights.
\newcommand{\reva}[1]{\textcolor{red}{#1}} % Define highlight color for reviewer 1
\newcommand{\revb}[1]{\textcolor{blue}{#1}} % Define highlight color for reviewer 2
```
The highlights can be hidden by changing to `\textcolor{black}{#1}`.


## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/) public domain, see `LICENSE` for more information.


## Acknowledgements

Largely based on:
>**Tiede ja Teksti: Tehoa ja taitoa tutkielman kirjoittamiseen.** / Kniivilä, Sonja; Lindblom-Ylänne, Sari; Mäntynen, Anne.
3., uudistettu painos toim. Helsinki: Gaudeamus, 2017. 250 s.
