## sf-t0000-mirroring-test
GitHub 2 GitLab mirroring test + GitHub Actions
<br/><br/>

### Usage

```
## ..locally

$ git clone https://github.com/VictorNuzhdin/sf-t0000-mirroring-test.git
$ cd sf-t0000-mirroring-test

$ mkdir -p .github/workflows/
$ cp action_example.yml .github/workflows/sync2gitlab.yml

$ echo "## sf-t0000-mirroring-test" >> README.md
$ echo "GitHub 2 GitLab mirroring test + GitHub Actions" >> README.md

$ git add .
$ git commit -m "First action for GitLab mirroring example"
$ git commit --amend
$ git commit -m "First action for GitLab mirroring example 1"
$ git push

## ..remotely on GitHub
##   https://github.com/VictorNuzhdin/sf-t0000-mirroring-test
check is files exists: README.md, action_example.yml, .github/workflows/sync2gitlab.yml (not showed in GitHub UI)

## ..remotely on GitLab
##   https://gitlab.com/drvicx-skillfactory/sf-t0000-mirroring-test
check is files exists: README.md, action_example.yml, .github/workflows/sync2gitlab.yml (showed in GitLab UI)

```
