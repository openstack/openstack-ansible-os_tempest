os_tempest role
###############
:tags: openstack, cloud, ansible, os_tempest
:category: \*nix

os_tempest Role

.. code-block:: yaml

    - name: os_tempest role
      hosts: "hosts"
      user: root
      roles:
        - { role: "os_tempest" }
