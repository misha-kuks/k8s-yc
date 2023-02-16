# k8s-yc
Deployment k8s cluster in yandex cloud
Include terraform manifest and ansible tasks/
Create k8s cluster on 2 nodes, 1 master, 1 worker.
To run follow:
1. Create your own file terraform.tfvars file which include your cloud_id,folder_id and yc_token.
2. terraform init
3. terraform apply
Terraform manifest create inventory file for ansible.
Wait 5 minutes, because type of vm disks is hdd, it's so slow.
4. ansible-playbook k8s_start.yml
Checkout:
5. ssh ubuntu@external_ipv4_address_kubermaster.
6. ![image](https://user-images.githubusercontent.com/117683403/219477704-bb227ad8-8db1-43c6-84c8-c8e947f758f1.png)
