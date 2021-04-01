Создано на основе:

    https://kubernetes.io/blog/2019/03/15/kubernetes-setup-using-ansible-and-vagrant/

Но есть правки:
для файла /etc/default/kubelet в ansible прописываем
create: yes

и для calico используем более новыую верию файла:
    Вместо:  command: kubectl create -f https://docs.projectcalico.org/v3.4/getting-started/kubernetes/installation/hosted/calico.yaml
    command: kubectl create -f https://docs.projectcalico.org/manifests/calico-typha.yaml