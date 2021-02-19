# Report

This repository is connected with Overleaf through [moritzgloeckl/overleaf-sync](https://github.com/moritzgloeckl/overleaf-sync).

```
ols login [-u/--username -p/--pasword --path]
ols [-l/--local-only -r/--remote-only --store-path -p/--path -i/--olignore]
```
Calling `ols` on itself will two-way sync with Overleaf. **Note that a merge will not happen automatically if the files are changed both locally and remotely, so ask in Slack if ever in doubt.**

If the local file is overwritten accidentally, just redo in your text editor. If the remote is overwtitten, have a look at _History_ on Overleaf.

> When modifying a file on Overleaf and immediately syncing afterwards, the tool might not detect the changes. Please allow 1-2 minutes after modifying a file on Overleaf before syncing it to your local computer.

The software flow chart can be compiled separately as a standalone, so it can be included elsewhere. To speed things up, `mode=buildnew` option on the `standalone` package means `--shell-escape` must be enabled.
