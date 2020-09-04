# GitHub Action: Idea Inspector

Cli tools for inspecting idea project

## Example
```yaml
name: "build-test"
on:
  push:

jobs:
  test_ci:
    runs-on: ubuntu-latest
    steps:
      - uses: lionzxy/idea-cli-inspector-actions@v1
```

## Run with CLI arguments

Full description you can find [here](https://github.com/bentolor/idea-cli-inspector)

```yaml
name: "build-test"
on:
  push:

jobs:
  test_ci:
    runs-on: ubuntu-latest
    steps:
      - uses: lionzxy/idea-cli-inspector-actions@master
        with:
          args: -v -rf pom.xml -p inspectionprofile.xml
```
