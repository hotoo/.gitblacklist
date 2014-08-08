
# GIT blacklist checker

----

GIT - pre-commit check and reject certain words/phrases/functions
commit into git repository.


## Install

```bash
$ npm install gitblacklist -g
```

## Usage

```
$ gitblacklist init
```

## Configuration

`gitblacklist` use following blacklist files to definition blacklist for
certain words/phrases/functions.

* `REPO_ROOT/.gitblacklist.[ext]`
* `REPO_ROOT/.gitblacklist`
* `~/.gitblacklist.[ext]`
* `~/.gitblacklist`

description:

* `REPO_ROOT/.gitblacklist.[ext]` and `~/.gitblacklist.[ext]` is for
    specifically filetype.
* `.gitblacklist` and `~/.gitblacklist` is for all of files.
* `REPO_ROOT/.gitblacklist.[ext]` and `REPO_ROOT/.gitblacklist` is for
    current repository.
* `~/.gitblacklist.[ext]` and `~/.gitblacklist` is for all of current user's
    repository.

Pre-line a certain words/phrases/functions.

## Example

To check for "TODO" or "FIXME" in a java file, create the file `{REPO_ROOT}/.gitblacklist.java` containing the two lines:

```
TODO
FIXME
```


## Bugs

For any bugs, please visit
[issues](https://github.com/hotoo/.gitblacklist/issues)
