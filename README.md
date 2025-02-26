# Team Optimal First Report

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This repository is connected with Overleaf through
[moritzgloeckl/overleaf-sync](https://github.com/moritzgloeckl/overleaf-sync)
and [eleanor-clifford/ols-git-tools](https://github.com/eleanor-clifford/ols-git-tools)

The software flow chart can be compiled separately as a standalone, so it can
be included elsewhere. To speed things up, `mode=buildnew` option on the
`standalone` package means `--shell-escape` must be enabled.

Style files for [Tikzit](https://tikzit.github.io) are also included, see
`flowchart/tikzit_example.tex` for way to compile `.tikz` files as a standalone
so it can be compiled and imported into the main report the same way. Please
keep 6 units around decision blocks, and 3 or 4 between other blocks. Also do
not use any special characters in the names of `.tikz` files, or LaTeX will
complain.

## Overleaf Integration

To set up the overleaf integration, install
[overleaf-sync](https://github.com/moritzgloeckl/overleaf-sync) and log in with
```
ols login [-u/--username -p/--pasword --path]
```
note that ols requires that the name of your folder is the same as the name of
the project on overleaf, so you will have to rename this folder to `idp_report`
locally.

Next run the following from any Linux/MacOS terminal, or Git Bash on Windows
```
git submodule update --init
./ols-git-tools/setup.sh
```

You can now use `git sync` to merge the overleaf changes into git. Note that
the automatic merge may not achieve your goals (it forces a conflict) but you
can manually compare the changes with `git diff HEAD~`

Also note (from the
[overleaf-sync](https://github.com/moritzgloeckl/overleaf-sync) docs):

> When modifying a file on Overleaf and immediately syncing afterwards, the
> tool might not detect the changes. Please allow 1-2 minutes after modifying a
> file on Overleaf before syncing it to your local computer.

## License

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
