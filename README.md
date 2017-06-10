# gtan-docker
Docker image for GTA Network servers

## Using

GTA Server root lies at `/srv`. It does *not* contain an example resource.

Quick and dirty example
```bash
$ docker run -d \ 
  -v"$(pwd)/resources:/srv/resources" \
  -v"$(pwd)/settings.xml:/srv/settings.xml" \
  -p"4499:4499/udp" \
  katie/gtan
```

See https://github.com/kayteh/rush for an example of how to use this for production.

## Updating

Make a PR with the VERSION file changed to the new version. It's that simple.
