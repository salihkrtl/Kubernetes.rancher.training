@salihkrtl ➜ /workspaces/Kubernetes.rancher.training (main) $ helm repo update
Error: no repositories found. You must add one before updating

Çözüm
@rifaterdemsahin ➜ /workspaces/helm (main) $ helm repo add stable https://charts.helm.sh/stable "stable" has been added to your repositories

@rifaterdemsahin ➜ /workspaces/helm (main) $ helm repo update Hang tight while we grab the latest from your chart repositories... ...Successfully got an update from the "stable" chart repository Update Complete. ⎈ Happy Helming!⎈he