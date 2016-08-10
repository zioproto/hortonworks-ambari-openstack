# Readme

## Create a Ubuntu VM in Openstack to run diskimage-builder

Create your config file:

```
cp vars.yaml.template vars.yaml
```

Source your openstack config:

```
source ~/openrc
```

Run the playbook

```
export ANSIBLE_HOST_KEY_CHECKING=False
ansible-playbook main.yaml
```
Check the public IP address of the ambari1 server

```
openstack server list
```

Point your browser to http://ambari1:8080

Login as `admin` password `admin`

![Install Options Screen](docs/ambari1.tiff)
