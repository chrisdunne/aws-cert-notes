### IAM

- Policy Simulator: allows you test IAM permissions, before deploying to production.
- Validate Policies: test policies behave in the way they were intended too.
- Test Attached Policies: ensure users, groups, and roles have the correct permissions.
- https://policysim.aws.amazon.com/

- USERS, GROUPS, AND ROLES.

- IAM IS GLOBAL, NOT REGIONAL.

- Root account is the account you initially setup with AWS.

- New users have no permissions at all when created.

- New users are assigned `Access Key ID` and `Secret Access Key` when the account is created.

- The `Access Key ID` and `Secret Access Key` are used for programmatic access and cannot be used to log into the AWS Console.

- A file can be downloaded with your `Access Key ID` and `Secret Access Key` ONCE, you can still view your `Access Key ID` but if you were to lose the `Secret Access Key` you would need to generate a new one.

- Always set up MFA on the root account.

- Always set up a password rotation policy.
