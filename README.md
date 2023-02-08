# User-Remove

A role to remove a user. By default does not remove directories associated with the user, but that's an option.

## Requirements

Sudo access to the server. 

## Required variables

Required variables are listed here, along with default example values. Any of these defaults can be overwritten by using the vars role directory. 

    username: tempuser

This is the name of the user to remove.

    delete_dir: false

Whether to delete directories associated with the user or not.

## Dependencies

None.

## Example Playbook

    - name: Remove the user account.
      hosts: linux
      become: true
      roles:
        - role: user-remove

### License

MIT

### Author Information

Derek Smiley - Network Analyst, avid homelabber, and aspiring Systems Administrator.
