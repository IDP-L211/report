# Report

This repository is connected with Overleaf through
[moritzgloeckl/overleaf-sync](https://github.com/moritzgloeckl/overleaf-sync)
and [eleanor-clifford/ols-git-tools](https://github.com/eleanor-clifford/ols-git-tools)

```
ols login [-u/--username -p/--pasword --path]
ols [-l/--local-only -r/--remote-only --store-path -p/--path -i/--olignore]
```
note that ols requires that the name of your folder is the same as the name of
the project on overleaf, so you will have to rename this folder from `report`
to `idp_report` locally.

Setup the git tools by running the following from any Linux/MacOS terminal, or
Git Bash on Windows
```
git submodule update --init
./ols-git-tools/setup.sh
```
Only run the setup script once, as there is currently no logic to detect if you
have already executed this command. If you mess it up and it breaks, remove the
duplicates from `.git/config`.

You can use `git sync` to merge with overleaf. Note that the automatic merge
may not achieve your goals, but you can manually compare the changes with
```
git diff HEAD~
```

Also note:

> When modifying a file on Overleaf and immediately syncing afterwards, the
> tool might not detect the changes. Please allow 1-2 minutes after modifying a
> file on Overleaf before syncing it to your local computer.

The software flow chart can be compiled separately as a standalone, so it can
be included elsewhere. To speed things up, `mode=buildnew` option on the
`standalone` package means `--shell-escape` must be enabled.
