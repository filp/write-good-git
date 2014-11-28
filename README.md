# write-good-git

Write more good commit messages, using [write-good](https://github.com/btford/write-good), a naive
linter for English prose, and a simple git hook.

![](http://i.imgur.com/PQe2mTf.png)


## Requirements

- Git
- Node and npm

## Getting started

- Install write-good globally:

    `$ npm install -g write-good`

- Clone this repository somewhere:

    `$ git clone https://github.com/filp/write-good-git.git`

- In the project you wish to use `write-good-git`, copy the hook to your `.git/hooks` directory.

    `$ cp ../write-good-git/git/hooks/commit-msg .git/hooks`

- Done! Next time you commit on that project, you'll get warnings from `write-good` (if you don't write so good).


## Configuration

`write-good-git` accepts configuration through environment variables:

- `WRITE_GOOD_PATH`: path to the location of the `write-good` executable
- `WRITE_GOOD_GIT_ALLOW`: if defined, `write-good-git` will NOT cancel the commit if any errors are present


## Authors

`write-good-git` was created by [Filipe Dobreira](https://github.com/filp). Most of the heavy-lifting comes
from Brian Ford's [write-good](https://github.com/btford/write-good) library.
