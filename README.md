# kustomize-issue-4958

To reproduce:

```
kustomize build --enable-alpha-plugins example/
```

The image in `config.yaml` doesn't matter to reproduce the issue as the bug happens before the image is fetched.
