# Features
- multiple additional `FROM` statements
- extract artifacts from previous stage
- combine multiple Dockerfiles into single as stages
- stop at (build) a specific build stage
- whichever `FROM` statement is last, is final base image

```bash
~/disk/E/workspace/github.com/toransahu/docker-eg/multi-stage-build on  main! ⌚ 23:08:01
$ docker image build -t toransahu/multi-stage-eg:v0.0.1 .
$ docker run --entrypoint "/bin/sh" -it toransahu/multi-stage-eg:v0.0.1

# stop at (build1) a specific build stage
$ docker build --target build1 -t toransahu/multi-stage-build1:v0.0.1 .
```
