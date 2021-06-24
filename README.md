# Morpheus Images Test Drive

## Quickstart

Put your Morpheus URL and API key into `group_vars/all` or supply them on the command line with `ansible-playbook`

Now run:
```
ansible-galaxy install -r requirements.yml --roles-path=roles/
ansible-playbook -i inv build_testdrive.yml
```

Morpheus Test Drive Builds should now be available and featured in Morpheus.