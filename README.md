# PRL cluster config

## Running playbook

```sh
ansible-playbook -i hosts site.yml
```

## Structure

```txt
.
├── group_vars
│   └── all               - variables shared accross nodes
├── hosts
├── host_vars             - variables for each node
│   ├── prl3
│   └── prl4
├── roles
│   └── common           - packages, users, sudo, ... 
│       └── tasks
│           └── main.yml
└── site.yml
```

## Resources

- [Ansible best practices](https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html)
