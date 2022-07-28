# Action to build multiarch images

## Usage

Inside your github action, create this step
```yaml
    steps:
      
      - name: Using action to build multiarch image
        uses: Synqrinus/docker-build@v1
        with:
            ecr-repository:        # AWS ECR repository identifier
            image-tag:             # Desired image tag
            context:               # (OPTIONAL) Build context (default - '.' )
            build-args:            # (OPTIONAL) Build arguments
            platforms:             # (OPTIONAL) Platforms list (default - 'linux/amd64,linux/arm64' )
            aws-access-key-id:     # AWS access key ID
            aws-secret-access-key: # AWS secret key
            aws-region:            # (OPTIONAL) AWS Region (default - 'us-west-2')
```
