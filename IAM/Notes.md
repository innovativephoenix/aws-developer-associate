## What is IAM?

# Stands for Identity and Access Management.

* Web service that helps the user securely control access to AWS resources.

* Used to control who is authenticated and authorized to use AWS resources.

* The first "identity" is the creation of account in AWS portal.  On providing the email and password an Identity is created, and that's the "root user" holding all the permissions to access all resources in AWS.

* The primary resources in IAM are users, groups, roles, policies, and identity providers.

* IAM Group is a collection of IAM Users. You use groups to specify permissions for a collection of users, which can make those permissions easier to manage for those users.


## Main things to remember:

1. IAM roles are like IAM Users in that they are both identities with permission policies that determine what the owner can access.

1. IAM Role do not have any credentials associated with them.

1. IAM Roles are is intended to be assumable by anyone who needs them.

1. IAM can be used from the AWS CLI, AWS SDK and AWS Management Console
