# Ansible Collection Skeleton

Collection template repository.

*This* readme file should contain a the name and a short description/quick docs of the collection and an optional 
link to `docs/` for more complete documentation.

Current directory structure:

* `docs/`: local documentation for the collection
* `license.txt`: optional copy of license(s) for this collection
* `galaxy.yml`: source data for the `MANIFEST.json` that will be part of the collection package
* `playbooks/`: playbooks reside here tasks/: this holds 'task list files' for include_tasks/import_tasks usage
* `plugins/`: all ansible plugins and modules go here, each in its own subdir
* `modules/`: ansible modules
* `lookups/`: lookup plugins
* `filters/`: Jinja2 filter plugins
... rest of plugins
* `README.md` or `README.rst`: this file
* `roles/`: directory for ansible roles
* `tests/`: tests for the collection's content

## Dependencies

Setup roles:

```shell script
ansible-galaxy role install -r requirements.yml -p ./roles
```

Setup collections:

```shell script
ansible-galaxy collection install -r requirements.yml -p ./collections
```

## Playbooks

Install plays:

```shell script
ansible-playbook site.yml -K
```

Uninstall plays:

```shell script
ansible-playbook purge.yml -K
```

Backup plays:

```shell script
ansible-playbook backup.yml -K
```

Restore plays:

```shell script
ansible-playbook restore.yml -K
```