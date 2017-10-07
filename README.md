Ansible role steamcmd
=====================

Setup and install the Steam command-line client.
This client is used to manage your Steam dedicated servers.

> Note that for Steam Guard, you should probably login once "by hand" first to generate a code.

Role Variables
--------------

```
steamcmd_create_user: true # create a dedicated user for the steam cmd
steamcmd_user: steam # owner of the steam cmd
steamcmd_user_home: /home/{{ steamcmd_user }}/ # home directory of the owner
steamcmd_directory: /home/{{ steamcmd_user }}/cmd/ # install directory of the cmd
steamcmd_login_timeout: 120
steamcmd_steam:
  username: anonymous # steam username
  password: ~ # steam password
  guard: ~
```

Example Playbook
----------------

```
- hosts: servers
  roles:
    - steamcmd
```

License
-------

MIT

Links
-----

<https://developer.valvesoftware.com/wiki/SteamCMD>
