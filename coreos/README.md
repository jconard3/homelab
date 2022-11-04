# Generating Ignition file from Butane config
```
$ podman run --interactive --rm quay.io/coreos/butane:release --pretty --strict < k8s-node.bu > k8s-node.ign
```

# Installing CoreOS from Generated Ignition file
```
$ sudo coreos-installer install /dev/sda \
  --ignition-url https://raw.githubusercontent.com/jconard3/homelab/master/coreos/ignition/k8s-node.ign
```

# Installing K8s
```
$ curl -LO https://raw.githubusercontent.com/jconard/homelab/master/coreos/install-k8s.sh && \
    bash install-k8s.sh
```
