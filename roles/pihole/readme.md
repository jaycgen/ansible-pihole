This role uses an ansible vault encrypted value

# Initialise a new vault password for pihole_webpassword
`ansible-vault encrypt_string --vault-id dev@prompt --stdin-name 'pihole_webpassword'`

# Append the ask-vault-pass flag to playbook runs
`ansible-playbook -i your_inventory your_playbook.yml --ask-vault-pass`
