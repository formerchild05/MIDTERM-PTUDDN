Mỗi khi push version mới của code github actions sẽ chạy CI và build image đẩy lên docker hub
![img_1.png](img_1.png)

Config argoCD
![img_2.png](img_2.png)

đợi pull image ![img_3.png](img_3.png)


monitor app đã deploy
![img_4.png](img_4.png)

chạy `kubectl apply -f cpu-alert.yaml`
![img_5.png](img_5.png)

`kubectl create secret generic alertmanager-prometheus-kube-prometheus-alertmanager -n monitoring --from-file=alertmanager.yaml=alertmanager.yaml --dry-run=client -o yaml | kubectl apply -f -`
apply message slack


cho Jmeter chạy với 50 thread
![img_6.png](img_6.png)

alert chạy
![img_7.png](img_7.png)