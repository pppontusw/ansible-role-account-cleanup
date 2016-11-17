## Delete accounts, sudoers or just ssh keys from servers.

Specify these in your hosts variables and run the role

```
# ssh keys to remove
clear_ssh_keys:
  - name: test
    pubkey: ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDchf70YBcTrTIPhiLkLyN7UgnFXuo62bg0bwkRi1S/3ePOJumX3HCVNUPmZ2J9Whx6k43A9I36NjViAu/ujakrHG+turemS+9GE9Zw0Re77J+fkiGOOgJG0yhP0SraZ1pDdzjCPJpqukb9gUbQIdOprGT4shxb8xTpUHUiQHsjvV8mJoB7qlYAvJqWYwexqJ3f75FZA5tjbPWXyTCkrjU4TbfsAXsk3N30ikExxmRVq0AK3fhIK/mo/Xx8pSaBi9DvLaVyzs9ioIjRaoAAuck0PXZs+BDiqwx0hUeeu4DpyygoE8uceI08etGjkTc3Wl6aww07u2zfkj+E9gNhfZxT pc@sto1-ansible

# accounts to remove from sudoers
clear_sudoers:
  - test

# accounts to remove altogether
clear_accounts:
  - test
```