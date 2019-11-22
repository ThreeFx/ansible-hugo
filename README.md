hugo
=========

Sets up "CD" for a hugo site hosted on git.

Requirements
------------

None.

Role Variables
--------------


| Variable Name | Default Value | Description |
--------------- |---------------|--------------
`hugo_user` | "hugo" | User to run hugo as (will be created if not present)
`hugo_home` | "/home/hugo" | Home directory of the hugo user
`hugo_minify` | True | Whether to minify the generated content.
`hugo_render_drafts` | False | Whether to render content marked as draft
`hugo_dir` | "/var/www/hugo" | Directory to clone the hugo repo to
`hugo_root` | "/" | Relative path in the repo where to run hugo
`hugo_repo` | "changeme" | **required**, the repository to check out
`hugo_repo_version` | "master" | Git branch/tag/hash to clone
`hugo_repo_ssh_key` | "changeme" | **required if `hugo_repo` cloned via ssh** SSH key with whom to pull the hugo repository

Dependencies
------------

None.

Example Playbook
----------------

See `molecule/default/playbook.yml`.

License
-------

BSD

Author Information
------------------

Find me on [GitHub](https://github.com/ThreeFx).
