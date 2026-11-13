# publish-private-image-fixture

Test repository for "Publish your app" with a **private** container image.

The repository is public, but `docker-compose.yml` names
`ghcr.io/3-torus/publish-private-image:6.7.1`, a private copy of podinfo 6.7.1.
Without a saved registry login for ghcr.io, publishing must be refused with
"this image needs a login: save a registry login for ghcr.io in Settings".
With a read:packages login saved, it must publish, test and deploy.
