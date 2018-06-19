Ansible Role Skeleton
=====================

This is a revisited version of the skeleton role [shipped with
Ansible](https://github.com/ansible/ansible/tree/devel/lib/ansible/galaxy/data/default).
Its purpose is to speed-up the bootstraping of a new role and it has the
following additional features:

- Includes ready-made CircleCI configuration template, with
  efficient caching policy (most reasonably sized role build
  should last under 30s.);
- Includes ready-made local testing framework to test your
  role within a docker container [1];
- Provides requirements to quickly create a new virtualenv
  if need be;

And improves on the following:

- Improves on the provided [TravisCI](https://travis-ci.org)
  configuration file: includes linting, running the test playbook;


No more excuse for not testing your roles !

Finally, it might not please your taste, it also include
customized README, etc. templates. Well fell free to
[fork](https://github.com/cans/role-template#fork-destination-box)



[1] depends on the [chrismeyersfsu.provision_docker](https://galaxy.ansible.com/chrismeyersfsu/provision_docker)
