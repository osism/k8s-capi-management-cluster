# k8s-capi-management-cluster

A [management cluster](https://cluster-api.sigs.k8s.io/user/concepts.html#management-cluster)
is required to use Kubernetes [Cluster API](https://cluster-api.sigs.k8s.io). With the Ansible playbook
in this repository, this management cluster can be deployed on OpenStack cloud infrastructure.

## Installation

```
pipenv install
pipenv shell
ansible-galaxy install -r requirements.yaml
```

## Usage

```
ansible-playbook -i localhost, playbook-infrastructure.yaml
ansible-playbook -i localhost, playbook-bootstrap.yaml
```
