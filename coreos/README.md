# Generating Ignition file from Butane config
```
$ podman run --interactive --rm quay.io/coreos/butane:release --pretty --strict < k8s-node.bu > k8s-node.ign
```
