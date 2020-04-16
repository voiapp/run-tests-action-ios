# Run tests action for our apps


## Usage

```workflow

jobs:
  assignee_to_reviewer:
    runs-on: whatever-you-need
    steps:
      - name: Run test - [Production]
        uses: voiapp/run-tests-action-ios@VERSION-TAG
        with:
        environment: 'production'
        developer_dir: ${{ matrix.xcode }}

```

The environment variable takes either single environments (production, stage) or combined ones with a dash in between.
