# K8S-install

**Clone repository** 

    git clone https://github.com/kubernetes-sigs/kubespray.git

    apt install python3.10-venv
    
    python3 -m venv kubespray-venv

    source kubespray-venv/bin/activate

    pip install -r requirements.txt 

    cd kubespray/inventory

    cp -R sample mycluster

    ansible-playbook cluster.yml -i inventory/mycluster/inventory.ini

    scp root@95.217.5.17:/etc/kubernetes/admin.conf .

Delete Cluster k8s

    ansible-playbook reset.yml -i inventory/mycluster/inventory.ini
   
