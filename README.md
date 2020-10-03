### Github Action

##### Usage
```yaml
rules:
    name: Rules
    runs-on: ubuntu-latest
    steps:
      - name: Fetch Branch Name
        uses: aptyInc/gha-branch-name@0.1.0
        id: branch
      - name: Print branch Name
        run: echo "${{steps.branch.outputs.branch_name}}"
```