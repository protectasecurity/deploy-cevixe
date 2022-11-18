# Deploy Cevixe GitHub Actions

Deploy Cevixe GitHub Actions allows you to deploy cevixe projects

## Example usage

```yaml
on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: protectasecurity/deploy-cevixe@v1
        env:
          AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}
          AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
          AWS_DEFAULT_REGION: 'us-east-1'
```

## Environment

- `AWS_ACCESS_KEY_ID` **Required**
- `AWS_SECRET_ACCESS_KEY` **Required**
- `AWS_DEFAULT_REGION` **Required**

## Authors

- [Ronnie Ayala](https://github.com/ronnieacs)