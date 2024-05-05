Commands
========

The Makefile contains the central entry points for common tasks related to this project.

Syncing data to your remote drive
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* `make copy_data` will use `rclone copyto` to recursively sync files in `data/` up to `{{ cookiecutter.rclone_drive }}:{{ cookiecutter.rclone_path }}`.
* `make sync_data` will use `rclone sync` to recursively sync files from `{{ cookiecutter.rclone_drive }}:{{ cookiecutter.rclone_path }}` to `data/`.
