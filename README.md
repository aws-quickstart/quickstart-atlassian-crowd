# quickstart-atlassian-crowd
## Crowd Software Data Center on the AWS Cloud
`Deployment Guide:` https://aws-quickstart.github.io/quickstart-atlassian-crowd/


Use this Quick Start to deploy Crowd Data Center on the AWS Cloud.

Crowd enables you to manage users from multiple directories - Active Directory, LDAP, OpenLDAP or Microsoft Azure AD - and control application authentication permissions in one single location. Crowd Data Center is a self-managed solution that gives you high availability, performance at scale, and disaster recovery for uninterrupted access to Crowd for all your teams.

This Quick Start uses the [Atlassian Standard Infrastructure (ASI)](https://fwd.aws/xYyYy) as a foundation. You can choose to build a new ASI for your deployment or deploy Crowd into your existing ASI. You can also deploy Jira, Confluence and Bitbucket Data Center within the same ASI.

![Quick Start architecture for Crowd on AWS](https://d1.awsstatic.com/partner-network/QuickStart/datasheets/jira-arch-on-aws.9d422797475ea5bd5d38f009ca8c540736f5449e.png)

For architectural details, best practices, step-by-step instructions, and customization options, see the 
[deployment guide](https://fwd.aws/Wz3Qb).

### Network prerequisites

You need to create the required AWS networking infrastructure
(VPC, subnets) by using the [ASI Quick Start](https://fwd.aws/xYyYy), or by deploying Crowd with a new ASI.
For details, see the [deployment guide](https://fwd.aws/Wz3Qb). 

## Development notes

### Pre-commit hook

It is recommended that you install the hooks under `submodules/quickstart-atlassian-services/scripts/hooks/`; this will
ensure that the metadata tags in the templates are automatically updated on
commit. The simplest method of doing this is:

    git config --add core.hooksPath submodules/quickstart-atlassian-services/scripts/hooks/

Alternatively you can invoke
`submodules/quickstart-atlassian-services/scripts/hooks/update-tags.py`
manually.

## Atlassian support

This Quick Start's CloudFormation templates were developed by Atlassian, in collaboration with AWS. To report an issue or request a feature, you can [contact Atlassian directly](https://support.atlassian.com/contact/#/).

For additional Atlassian documentation on how to manage Quick Start deployments, see [Running Crowd in an AWS cluster](https://confluence.atlassian.com/x/9uOJOw).
