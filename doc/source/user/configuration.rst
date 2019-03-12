========================
os_tempest configuration
========================

This page shows all of the variables which can be set in order to control
the behaviour of `os_tempest` role and provides examples on how to do so.

For a list of all variables with a default value set, please, refer to
the `this page`_.

.. _this page: ./default.html


python-tempestconf
------------------
python-tempestconf is a tool which generates a `tempest.conf` file necessary
for Tempest execution. For more information about the tool, please,
`follow its official documentation <https://docs.openstack.org/python-tempestconf/latest/index.html>`_.

If you want `os_tempest` to execute `python-tempestconf`, prior to Tempest
execution in order to generate `tempest.conf` file, set
*tempest_use_tempestconf* variable to true:

.. code-block:: yaml

    tempest_use_tempestconf: true

More information about `python-tempestconf` arguments can
`be found here <https://docs.openstack.org/python-tempestconf/latest/cli/cli_options.html>`_.

The best way how to pass any arguments to `python-tempestconf` is using its
`profile feature <https://docs.openstack.org/python-tempestconf/latest/user/profile.html>`_.

`os_tempest` provides *tempest_tempestconf_profile* variable for setting
desired `python-tempestconf` arguments.
For example, if you wanted to define **debug** to *true*, **os-cloud** to
*demo* and override output of `python-tempestconf` to
`/my/location/tempest.conf`, it would be done by:

.. code-block:: yaml

    tempest_tempestconf_profile:
      debug: true
      os-cloud: demo
      out: /my/location/tempest.conf
