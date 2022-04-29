rhel_subscription
=========

Role responsável por fazer a subscrição (registro) no portal Red Hat do sistema operacional instalado no servidor de execução.

Requirements
------------

Usuário e senha com permissão de subscrição no portal Red Hat.

Role Variables
--------------

subscription_user: indica o usuário que deve ser utilizado para fazer a subscrição.
subscription_password: indica a senha referente ao usuário citado acima - ecriptada através do Ansible Vault

Dependencies
------------


Example Playbook
----------------

A execução deve ser feita no Ansible Tower:

  Ansible Tower
    Templates
    - rhel_subscription

License
-------

Icaro Tech

Author Information
------------------

Icaro Tech
