# pipeline
git multi-environment pipeline

## Manual Multi-Environment Deployment

The workflow in `.github/workflows/manual-multi-env-deploy.yml` is triggered manually
(`workflow_dispatch`). From the **Actions** tab, select **Manual Multi-Environment Deployment**,
click **Run workflow**, and choose one of `dev`, `test`, `staging` or `prod`. Only the job for the
selected environment runs, using the matching GitHub Environment (so any protection rules, such as
required reviewers on `prod`, are applied).
