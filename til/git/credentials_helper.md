# Store password to Git server

For every repository one can save the password and then it will not ask for it everytime: 

```
git config credential.helper 'store --file=/home/rox/repos/.git-credentials'
```

This credential file is per _server_ not per repository, so it can be shared by several repositories which are on the same server (i.e. one uses the same credentials for accessing them).