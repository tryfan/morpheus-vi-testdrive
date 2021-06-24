# Morpheus Images Test Drive

## Quickstart

Copy `group_vars/all.dist` to `group_vars/all`

Put your Morpheus URL and API key into `group_vars/all`

Now run:
```
ansible-galaxy install -r requirements.yml --roles-path=roles/
ansible-playbook -i inv build_testdrive.yml
```

Morpheus Test Drive Builds should now be available and featured in Morpheus.