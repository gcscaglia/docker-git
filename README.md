# docker-git

## What is docker-git?

docker-git is a unofficial docker image for a [git][1] client. docker-git is based on [Alpine linux][2] for simplicity and small footprint.

[1]: https://git-scm.com
[2]: https://alpinelinux.org

## How to use this image?

This image does not offer any services nor convenient entrypoints; This image sole purpose is to be used for [CI][1] deploy jobs, where the best deploy strategy is a `git pull`.

It could also be used interactively, but there is little benefit in doing so. I won't discuss details of how to archive that, but my sugestion is to write a simple bash-wrapper arround this image, like what is done for [compose][2].

[1]: https://en.wikipedia.org/wiki/Continuous_integration
[2]: https://github.com/docker/compose/blob/master/script/run/run.sh
