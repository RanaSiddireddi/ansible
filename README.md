# ansible


### This is still manual way of getting info
ansible all -i inventory -e ansible_user=centos -e ansible_password=DevOps321 -m shell -a "df -h"
ansible all -i inventory -e ansible_user=centos -e ansible_password=DevOps321 -m shell -a uptime


-i inventory file
-e extra or environment variavles
ansible_user : special varaible fpr user-name to use
ansible_password : special varaible fpr user-password to use
-m : name of the module

Ansible scripts are referred as playbooks and they are written using yaml

YAML - Yet another markup language

markup manguage : presentation language

Things to remember while learning yaml

```
    1. YAML is indentation specific
    2. YAML is all about dictionary, list and maps
    3. YAML files should always end with .yml or .yaml
```

# List

```
    # A list of tasty fruits
    - Apple
    - Orange
    - Strawberry
    - Mango
```

# Dictionary
    martin:
        name: Martin D'vloper
        job: Developer
        skill: Elite

# list and dict
    - martin:
        name: Martin D'vloper
        job: Developer
        skills:
            - python
            - perl
            - pascal
    - tabitha:
        name: Tabitha Bitumen
        job: Developer
        skills:
            - lisp
            - fortran
            - erlang

# Map : a key with multiple keyvalue pairs

# playbook is list of plays. Play is list of tasks. task is list of action to execute
