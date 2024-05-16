# kubectl-k8s

Learn how to use `microk8s kubectl` directly as `kubectl` using `snap`.

## Install kubectl

Run the following command to install `kubectl`.

```bash
sudo snap install kubectl --classic
```

## Create the configuration for kubectl

```bash
cd $HOME
mkdir .kube
cd .kube
microk8s config > config
```

## Fix the configuration

It is possible that the IP address for the `cluster.server` in `config` file to be wrong.
In case you get an error when you execute the kubectl command, just replace the IP from there with `127.0.0.1`.

## Check if it works

Run the following command:

```bash
kubectl version
```
