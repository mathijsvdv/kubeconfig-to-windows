# kubeconfig-to-windows
Utility script to write the kubeconfig in WSL to the Windows folders so that Lens can connect to the cluster 

## Install
Download the shell script to $HOME/.local/bin to make it available anywhere in WSL:
```bash
wget https://raw.githubusercontent.com/mathijsvdv/kubeconfig-to-windows/master/kubeconfig-to-windows -O kubeconfig-to-windows
mv kubeconfig-to-windows $HOME/.local/bin/
chmod +x $HOME/.local/bin/kubeconfig-to-windows
```
