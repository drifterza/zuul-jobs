Install javascript dependencies needed for a project

**Role Variables**

.. zuul:rolevar:: zuul_work_dir
   :default: {{ zuul.project.src_dir }}

   The directory to work in.

.. zuul:rolevar:: tox_constraints_file

   Path to a pip constraints file. Will be provided to via
   ``TOX_CONSTRAINTS_FILE`` (deprecated but currently still supported
   name is ``UPPER_CONSTRAINTS_FILE``) environment variable if it
   exists.
   Useful if npm ``postinstall`` runs tox.
