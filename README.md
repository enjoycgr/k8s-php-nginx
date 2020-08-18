# k8s-php-nginx

## k3s
1. 安装docker
2. 安装k3s server： curl -sfL https://docs.rancher.cn/k3s/k3s-install.sh | INSTALL_K3S_MIRROR=cn INSTALL_K3S_EXEC="server --docker" sh
3. 安装k3s node:
    1. cat /var/lib/rancher/k3s/server/token
    2. curl -sfL https://docs.rancher.cn/k3s/k3s-install.sh | INSTALL_K3S_MIRROR=cn INSTALL_K3S_EXEC="--docker" K3S_URL=https://masterip:6443 K3S_TOKEN=token sh -
4. 卸载server：/usr/local/bin/k3s-uninstall.sh
5. 卸载node: /usr/local/bin/k3s-agent-uninstall.sh


