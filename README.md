# .github

## GitHub identity

GitHub identity is used to deploy the canisters to the Internet Computer from the GitHub Actions.

### Setup GitHub identity secret
1. Create a personal access token with the `admin:org` scope named `TEMP_PAT`
2. Run the `setup-identity` workflow
3. The workflow will create a new identity and set the identity PEM as an organization secret named `IDENTITY_PEM`
4. Delete `TEMP_PAT` token
5. Disable the `setup-identity` workflow to avoid over-writing the secret