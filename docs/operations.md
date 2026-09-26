# Operations guide

## Running the sample
Run `npx ts-node src/sample-output.ts` to print the output label.

## Checking the version
The displayed version is stored in `version.txt`.

## Troubleshooting

### Training Failure workflow fails at "Check output label"

**Symptom:** the Training Failure workflow fails in job `check-label`, at step **Check output label**, with:

```text
ERROR: expected output label 'Packet Sample' but src/sample-output.ts contains 'Packet Sampel'
```

**Remedy:** set `outputLabel` in `src/sample-output.ts` to `"Packet Sample"`, commit the fix on a branch, open a pull request against `main`, then rerun the Training Failure workflow from the Actions tab.
