# Morpheus Images Test Drive

## Quickstart

Put your Morpheus URL and API key into `group_vars/all` or supply them at runtime  on the command line.  
eg. 
```
ansible-playbook -e "@morpheuscreds.yml"
```

Now run:
```
ansible-galaxy install -r requirements.yml --roles-path=roles/
```

Here are the size requirements in your `/var/opt/morpheus/morpheus-ui` directory for each image set:

- VMWare: 5.5GB
- Azure: 25GB

Choose your image set and use the file as extravars.  For Azure:
```
ansible-playbook -i inv -e "@imagesets/azure.yml" build_testdrive.yml
```

Morpheus Test Drive Builds should now be available and featured in Morpheus.