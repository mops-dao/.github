# .github

## GitHub identity

- Principal: `6btvq-iqtba-hqxjf-t3qsx-ibayx-rkdgt-347cw-k6rqq-wf53n-6n47v-5ae`
- Generated: https://github.com/mops-dao/.github/actions/runs/16238244358

GitHub identity is used to deploy the canisters to the Internet Computer from the GitHub Actions.

### Setup GitHub identity secret
1. Create a personal access token with the `admin:org` scope named `TEMP_PAT`
2. Run the `setup-identity` workflow
3. The workflow will create a new identity and set the identity PEM as an organization secret named `IDENTITY_PEM`
4. Delete `TEMP_PAT` token
5. Disable the `setup-identity` workflow to avoid over-writing the secret