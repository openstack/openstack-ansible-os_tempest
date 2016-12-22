=================================
OpenStack-Ansible os_tempest role
=================================

This is the Ansible role to deploy OpenStack Tempest.

:tags: openstack, cloud, ansible, os_tempest
:category: \*nix

Basic role example
~~~~~~~~~~~~~~~~~~

.. code-block:: yaml

    - role: "os_tempest"
      ROLE_VARS...

To clone or view the source code for this repository, visit the role repository
for `os_tempest <https://github.com/openstack/openstack-ansible-os_tempest>`_.

Default variables
~~~~~~~~~~~~~~~~~

.. literalinclude:: ../../defaults/main.yml
   :language: yaml
   :start-after: under the License.

Required variables
~~~~~~~~~~~~~~~~~~

None

Example playbook
~~~~~~~~~~~~~~~~

.. literalinclude:: ../../examples/playbook.yml
   :language: yaml
