## Secrets

This project uses Bitwarden Secrets Manager to store and access secrets.

In order to connect to access the secrets, the application needs a secret with a access token, which can be created in the Secrets Manager web page.

```bash
kubectl create secret generic bw-auth-token -n henshi --from-literal=token=<access_token>
```