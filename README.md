# Convenienthy - Yet Another Implementation of `Conventional Commits`[^conventional-commits] (for Git) (in Python)

This code is **_heavily_** inspired on @craicoverflow [post](https://dev.to/craicoverflow/enforcing-conventional-commits-using-git-hooks-1o5p) at dev.to. Also check his solution approach: [Sailr](https://github.com/craicoverflow/sailr).

# Install

> ## Requiriments
>
> - Git CLI installed
> - Python 3.8+

## For All repositories in your account

1. Clone this repo to somewhere: `git clone https://github.com/theoamonteiro/conventional-commits.git ${somewhere}`
2. Set Git Templates folder to `${somewhere}`: `git config --global init.templatedir ${somewhere}`
3. Commit way!

# Configurations

## Ignore Repos

We projected 2 ways to ignore repos:

1. Set up the `enabled` property to `false` on the `.conventional-commits.json` file at the root of the repository
2. Create a file `.no-conventional-commits` at the root of the repository (`touch .no-conventional-commits`)

> **IMPORTANT**: `.no-conventional-commits` takes precedence over `.conventional-commits.json`.

# Notes & References

[^conventional-commits]: See _Conventional Commits 1.0.0_ - https://www.conventionalcommits.org/en/v1.0.0/
[^.gittemplates]: There are some inclination towards `~/.git-templates` (or `~/.git_templates`), see https://dev.to/craicoverflow/enforcing-conventional-commits-using-git-hooks-1o5p and https://craftquest.io/articles/using-custom-templates-in-git-to-change-the-default-branch-name and https://git-template.readthedocs.io/en/latest/