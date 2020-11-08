========

Azure Storage Blob Download Blob

Requirements
------------

Must have exported Azure Storage environment variables defined below in the ansible host environment.
In AWX, ensure Azure account is attached to project template when created or launched.

A valid Azure Storage Blob must be defined in the project.  

Role Variables
--------------

AZURE_CLIENT_ID - environment variable
AZURE_SECRET - environment variable
AZURE_SUBSCRIPTION_ID - environment variable
AZURE_TENANT - environment variable
AZURE_RESOURCE_GROUP - environment variable
AZURE_STORAGE_ACCOUNT - environment variable
AZURE_BLOB_CONTAINER - environment variable
blob_file - template variable.  use job template to define.  Cannot be a list of multiple files.
project - template variable.  user job template to define.  Needs to be a complete folder path, as this will only act upon individual files.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      roles:
         - { role: ansible-role-azblobget }

License
-------

BSD

Author Information
------------------

This role was created by Dan Rodden