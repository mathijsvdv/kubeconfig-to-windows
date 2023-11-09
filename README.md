# kubeconfig-to-windows
Utility script to write the kubeconfig in WSL to the Windows folders so that Lens can connect to the cluster 

## Install
Download the shell script to $HOME/.local/bin to make it available anywhere in WSL:
```bash
curl https://raw.githubusercontent.com/mathijsvdv/kubeconfig-to-windows -o kubeconfig-to-windows
mv kubeconfig-to-windows $HOME/.local/bin/
chmod +x $HOME/.local/bin/kubeconfig-to-windows
```
