Ansible Role Skeleton
=====================


This is a revisited version of the skeleton role `shipped with
Ansible <https://github.com/ansible/ansible/tree/devel/lib/ansible/galaxy/data/default>`_.
Its purpose is to speed-up the bootstraping of a new role and it has the
following additional features:

- Includes ready-made `CircleCI`_ configuration template, with
  efficient caching policy (most reasonably sized role build
  should last under 30s.);
- Includes ready-made local testing framework to test your
  role within a docker container [#]_;
- Provides requirements to quickly create a new virtualenv
  if need be (probably best if you want to run tests);

And improves on the following:

- Improves on the provided `TravisCI`_ configuration file:
  includes linting, running the test playbook;


No more excuse for not testing your roles !

Finally, though it might not fit your needs, it als include customized
README, etc. templates. Well fell free to
`fork <https://github.com/cans/role-template#fork-destination-box>`_


.. [#] Depends on the `chrismeyersfsu.provision_docker <provdocker>`_ role.

.. _circleci: https://circleci.com
.. _travisci: https://travis-ci.org
.. _prodocker: https://galaxy.ansible.com/chrismeyersfsu/provision_docker


