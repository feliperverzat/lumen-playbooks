rhel_backup
=========

Role responsável por realizar o download, instalação e configuração do agente de backup (Netbackup), bem como do certificado e de outros pacotes necessários.

Requirements
------------

Pacotes do Netbackup disponíves para download no repositório de arquivos.
Listagens de servidores que serão adicionadas para monitoração no /etc/hosts do servidor de execução.

Role Variables
--------------

HOSTS.REGION: parâmetro para indicar em qual dos datacenters deve ser executada a role.
HOSTS.FILE: aponta qual o arquivo de servidores deve ser adicionado no /etc/host de acordo com a região informada via parâmetro REGION.
MEDIASERVER_SP: hostnames relativos a São Paulo.
MEDIASERVER_RJ hostnames relativos ao Rio de Janeiro.
MEDIASERVER_CTB: hostnames realtivo a Curitiva.

Dependencies
------------

Templates bp_sp.j2, bp_rj.j2 e bp_ctb.j2

Example Playbook
----------------

A execução deve ser feita no Ansible Tower:

  Ansible Tower
    Templates
    - rhel_backup


License
-------

Icaro Tech

Author Information
------------------

Icaro Tech
