# Rick Roll Action
A useless action that will post a gif of Rick Astley's _Never Gonna Give You Up_ to issues or pull requests.

## Example Usage
The action is set up to run on pull requests and issues created in this repository, check out the [workflow](.github/workflows/rick-roll.yml). Feel free to open an issue as a demo.

```yml
on:
  issues:
    types:
    - opened
  pull_request:
    types:
    - opened

jobs:
  roll:
    runs-on: ubuntu-latest
    steps:
    - uses: duck-dynasty/rick-roll-action@v1
      with:
        chance: 5  # a 5% chance of including the gif
```
