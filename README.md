# kubeconfig-to-windows
Utility script to write the kubeconfig in WSL to the Windows folders so that Lens can connect to the cluster 

## Install
Download the shell script to $HOME/.local/bin to make it available anywhere in WSL:
```bash
wget https://raw.githubusercontent.com/mathijsvdv/kubeconfig-to-windows/master/kubeconfig-to-windows -O kubeconfig-to-windows
mv kubeconfig-to-windows $HOME/.local/bin/
chmod +x $HOME/.local/bin/kubeconfig-to-windows
```

## Usage
After installing, run the script using:
```bash
kubeconfig-to-windows
```

This will take the current config of your clusters, and copy it over to the equivalent Windows folder in %USERPROFILE%/.kube/config,
while prepending "\\wsl.localhost\Ubuntu" to the paths to the cluster certificate authority, client certificate and client key files, so that they become valid Windows paths. Subsequently, Kubernetes Lens (installed on Windows)
can pick up this kubeconfig file ('+' icon -> 'Select Kubeconfig file(s)') and connect to the clusters defined in it.
