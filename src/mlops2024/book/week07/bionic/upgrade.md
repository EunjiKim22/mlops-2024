# Upgrading Bionic

## Update the version and hashes

```yaml
apiVersion: bionic-gpt.com/v1
kind: Bionic
metadata:
  name: bionic-gpt
  namespace: bionic-gpt
spec:

  ...

  # Single Sign ON
  sso-secret: oidc-credentials

  ...

```

## Apply the new configuration
