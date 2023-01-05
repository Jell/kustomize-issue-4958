# kustomize-issue-4958

To reproduce:

```
kustomize build --enable-alpha-plugins example/
```

The image in `config.yaml` doesn't matter to reproduce the issue as the bug happens before the image is fetched.

Kustomize version 4.5.5+ fails with this error:

```
Error: couldn't execute function: chdir /tmp/kustomize-2734089145: no such file or directory
```
