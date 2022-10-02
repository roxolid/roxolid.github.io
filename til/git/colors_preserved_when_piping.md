# Preserve colors in Git output when piping to `head`, `less`, ...

Just alter the repository's `color.diff` configuration property to `always`:

```
git config color.diff always
```

Or globally for all repositories:

```
git --global config color.diff always
```
