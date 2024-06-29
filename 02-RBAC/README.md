# Configure Identity Provider & RBAC

## Step 1 - Create a htpasswd provider

Configure the htpasswd identity provider using the documentation below.
Create user with your own first name and a complex password.

https://docs.openshift.com/container-platform/4.14/authentication/identity_providers/configuring-htpasswd-identity-provider.html

## Step 2 - Custom role

Create a Custom role that only allows viewing secrets and config maps in your namespace

https://www.redhat.com/sysadmin/rbac-openshift-role

## Step 3 - Rolebinding

Assign the new role to a user from your htpasswd provider.

https://www.redhat.com/sysadmin/rbac-openshift-role

## Step 4 - test

Login with that user and check if everything is working.

## Step 5 - cluster admin

Now give the user also cluster-admin permissions

## Bonus

 Create a new role that allows for impersonating ONLY your own user and assign it to the test user.
