# Template repository

This is a template repository prepared for python-based projects in
[swinnoproject](https://github.com/swinnoproject).

Before your first commit I suggest that you:

1. Rename `/src/template/ `
2. Update `pyproject.toml`:

```
[3] name = "Template"`
[6] name="", email=""`
[8] description = ""`
[58] "src/template/" (to match the name from step 1)
```
3. Update `.github/workflows/auto_assign.yml`:
```
[16] repo-token: ${{ secrets.GITHUB_TOKEN }}
[17] assignee: USERNAME
```

4. Install pre-commit and:

   a. (Optionally) update `.pre-commit-config.yaml`, by default it will:
    - on commit:
        1. isort (sort imports)
        2. black (format code)
    - pre-push:
        1. Make sure that it passes all existisng pytests
        2. Remove trailing whitespaces
        3. Fix enf of files
        4. Check yaml files
        5. Check if any large files are added  by mistake.

    b. Initialize pre-commit for this repository

5. Change the contents in this file.
