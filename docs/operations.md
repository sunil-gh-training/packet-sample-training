# Operations guide

## Running the sample
Run `npx ts-node src/sample-output.ts` to print the output label.

## Checking the version
The displayed version is stored in `version.txt`.


## Deployments

Changes reach the training environment through the **Training Deployment** workflow, which runs on pushes to `main` and records a deployment to the `training` environment.

To check what is currently deployed:

1. Open the repository's **Deployments** page and select the `training` environment.
2. Open the most recent deployment record to see its status and source branch.
3. Follow that deployment to the commit it released to see the change it deployed.

The deployed sample marker is stored in `deployment-sample.txt`.
