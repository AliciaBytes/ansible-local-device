# ansible-local-devices

This repository contains ansible automation scripts.

## How to use

Install the dependencies with:

```sh
ansible-galaxy install -r requirements.yml
```

To run a playbook execute the following in a dev container:

```sh
ansible-playbook playbook.yml -K --check
```

The `--check` command is for a dry run and only checking what would be changed by running the playbook.

### Selectively running tasks

You can run only a selection of tasks by running it with `--tags selected_tag` or `--skip-tags unselected_task`.

Currently available tasks can be checked out with --list-tags

A possibly incomplete list of them:

- configuration
- general_settings
- users
