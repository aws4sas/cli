Conception. (DRAFT)


Unix System Administrators like to run commands to interrogate systems and platforms.

These commands usually have short names and easily memorable. Often their are flags.

This project is for admins that want to have a unix-like experience within AWS.


The AWS CLI is an excellent tool with one weakness. It's so rich in options that it can be hard to remember them all and we feel there is a place for a set of simple commands that sit in a place between the cli-minded user and the full AWS CLI tool. We're certain that many have already embarked on their own version of this so why do it all again ?

If we can achieve the following goals we will feel like we have accomplished something.

1. Enable users to quickly visualise an AWS environment through easy-to-remember CLI tools.
2. Enhance the accessibility of the CLI to new users, encouraging and accelerating their learning experience.


3. Provide an approach to the consistent naming of tools. Consider these possibilities "vpcstatus, vpc -status, status -vpc, vpcshow, vpclist". Let's use a consistent approach.

4. Script language selection. Where possible we should write scripts in Bash to avoid problems caused by Python versioning or lack of it.

5. Script support. We must agree some common functions so we don't "repeat ourselves".






Dont want to have to rename established commands.
There should be a naming methodology.


Example:
which of these do you find easier to remember ?
aws ec2 describe-route-tables --output text --query 'RouteTables[*].Associations[*].RouteTableId'
routelist
