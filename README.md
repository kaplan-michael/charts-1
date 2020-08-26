# one image - helm chart

    2019 Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/ondrejsika/one-image-helm

## Usage

Add repo

```
helm repo add ondrejsika https://helm.oxs.cz
```

Install

```
helm upgrade --install \
  <name> ondrejsika/one-image \
  --set image=<image> \
  --set host=<domain>
```

## Parameters

- `image` (default `ondrejsika/go-hello-world:2`) - Docker image you want to serve
- `host` (default `hello-world.local`) - Ingress hostname
- `www_redirect` (default `true`) - www alias with redirect
- `changeCause` (default `null`)
- `replicas` (default `1`)
