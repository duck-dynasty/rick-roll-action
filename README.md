# Rick Roll Action
A useless action that will post a gif of Rick Astley's _Never Gonna Give You Up_ to issues or pull requests.

## Example Usage
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
    - uses: twentylemon/rick-roll-action
      with:
        chance: 5  # a 5% chance of including the gif
```
