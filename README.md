# Redis automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-redis
  name: ansible-role-redis
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-redis

- Import role and override role variables, e.g.
```
- name: Setup redis
  roles:
    - role: ansible-role-redis
```

- All available role vars can be found in `defaults`
