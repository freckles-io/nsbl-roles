Default roles, included in the nsbl freckles connector.

This repository uses [frankentree](https://gitlab.com/frkl/frankentree) to manage it's sub-trees.

Ideally, child-repositories are only ever 'pulled' never pushed from this directory, as 'frankentree' cannot always handle all the cases that come up when pushing sub-trees.


Adding a new Ansible role is done with:

    frankentree add -u <role_url> <path>/<to>/<role>/<folder>/<role_name>

The path to the role should somehow describe the category of the role in question (e.g. system-tool, web-server, etc). If adding a 3rd-party role, it's best to fork it into the freckles-io-external organisation, then add it to this repository. That way changes can be pushed upstream if necessary.
