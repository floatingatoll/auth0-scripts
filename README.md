# auth0-scripts
Scripts to manage auth0 via API

It also includes other IAM related scripts, such as DuoSecurity scripts that may be useful in combination with IAM or Auth0.

# Scripts

## DuoSecurity
### duo_assign_groups.py
Automatically assign group to new users in Duo. This is used as a default Duo group for all users as Duo cannot do this
automatically.

## LDAP
### disable_deactivated_accounts.py
Automatically set Auth0 'ad' (LDAP) accounts to blocked ('disabled') if they are disabled in LDAP.

### ldap2s3
Uploads LDAP user profile data to an S3 bucket This allows easy access to user profiles in AWS, for example, for CIS.

### clearpass_disable_accounts.py
Automatically deletes users in Clearpass API (wifi) if they are disabled in LDAP or not part of the right group.
