# quickstart-atlassian-crowd
## Crowd Software Data Center on the AWS Cloud
For architectural details, step-by-step instructions, and customization options, see the [deployment guide](https://fwd.aws/g6Q3D).

To post feedback, submit feature ideas, or report bugs, use the **Issues** section of this GitHub repo. 

To submit code for this Quick Start, see the [AWS Quick Start Contributor's Kit](https://aws-quickstart.github.io/).

## Development notes

### Pre-commit hook

It is recommended that you install the hooks under `submodules/quickstart-atlassian-services/scripts/hooks/`; this will
ensure that the metadata tags in the templates are automatically updated on
commit. The simplest method of doing this is:

    git config --add core.hooksPath submodules/quickstart-atlassian-services/scripts/hooks/

Alternatively you can invoke
`submodules/quickstart-atlassian-services/scripts/hooks/update-tags.py`
manually.

## Deploying for production

For production deployments, avoid launching the Crowd Quick Start from the AWS Quick Start interface. If you do, any changes made to the Quick Start templates will propagate directly to your deployment. These updates sometimes introduce unexpected changes that could break your deployment.

Instead, clone the Crowd Quick Start templates to a custom Amazon Simple Storage Service (Amazon S3) bucket. Then, launch the templates directly from the S3 bucket. This practice lets you control when to apply the latest changes to your environment. See [Launching from a cloned Quick Start (recommended for production)
](https://aws-quickstart.github.io/quickstart-atlassian-crowd/#_launching_from_a_cloned_quick_start_recommended_for_production) for instructions.

## Atlassian support

This Quick Start's CloudFormation templates were developed by Atlassian, in collaboration with AWS. To report an issue or request a feature, you can [contact Atlassian directly](https://support.atlassian.com/contact/#/).

For additional Atlassian documentation on how to manage Quick Start deployments, see [Running Crowd in an AWS cluster](https://confluence.atlassian.com/x/9uOJOw).
