# Setup AWS Signer Notation CLI

A GitHub Action that installs and configures the AWS Signer Notation CLI on your GitHub runner. This action downloads, verifies, and installs the Notation CLI with AWS Signer plugin support.

## Usage
Add this action to your GitHub workflow:
```yaml
- name: Setup AWS Signer Notation CLI
  uses: rudderlabs/setup-aws-signer-notation-cli@v1
  with:
    public-key: ${{ secrets.AWS_SIGNER_PUBLIC_KEY }}
```

## Inputs

| Input | Description | Required |
|-------|-------------|----------|
| `public-key` | Public GPG key from AWS Signer used to verify the Notation CLI package signature | Yes |


## Related Resources
- [AWS Signer Documentation](https://docs.aws.amazon.com/signer/)
- [Notation Project](https://notaryproject.dev/)
- [Container Image Signing Best Practices](https://docs.aws.amazon.com/signer/latest/developerguide/Welcome.html)
