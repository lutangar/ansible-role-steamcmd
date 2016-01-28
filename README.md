# Ansible role steamcmd
Setup and install the Steam command-line client.
This client is used to manage your Steam dedicated servers.

## Usage
```
- hosts: myhostname
  roles:
    - steamcmd
```

## Defaults variables
```
steamcmd_create_user: true
steamcmd_user: steam
steamcmd_user_home: /home/{{ steamcmd_user }}/
steamcmd_directory: /home/{{ steamcmd_user }}/cmd/
steamcmd_steam:
  username: anonymous
  password: ~
```

## Links
<https://developer.valvesoftware.com/wiki/SteamCMD>

