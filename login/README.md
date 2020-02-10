## Required
- AWS CLI
- jq

## Preparation
- export AWS_ACCESS_KEY_ID="access key id for your account"
- export AWS_SECRET_ACCESS_KEY="secret access key for your account"

## Usage
```sh
source export-sts
```

Before
```sh
$ env | grep AWS
AWS_ACCESS_KEY_ID="access-key-id"
AWS_SECRET_ACCESS_KEY="secret-access-key"
```
↓

After
```sh
$ env | grep AWS
_AWS_ACCESS_KEY_ID="access-key-id"
_AWS_SECRET_ACCESS_KEY="secret-access-key"
AWS_ACCESS_KEY_ID="access-key-id for temporary-session-token"
AWS_SECRET_ACCESS_KEY="secret-access-key for temporary-session-token"
AWS_SESSION_TOKEN="temporary-session-token"
```
