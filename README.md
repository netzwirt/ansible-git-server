#git-server

Setup bare git-repositors on a server. 

#Role Variables

git_server_user_keys: list with users
git_server_repos: list with repos names
git_server_lookup_keys: path to users public keys

#Dependencies

None

#Example Playbook


    - hosts: git-server
      become: true
      vars:
		git_server_user_keys:
		- john
		git_server_repos:
		- foo
		- bar
		- baz
      roles:
         - { role: netzwirt.git-server }


#License

BSD

#Author Information

[netzwirt](https://github.com/netzwirt)

