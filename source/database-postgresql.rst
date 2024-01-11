##########
PostgreSQL
##########

PostgreSQL (or Postgres) is an open-source relational database. We provide binaries ready to start your own instance.

Refer to the `UberLab guide <https://lab.uberspace.de/en/guide_postgresql.html>`_ for details.


Versions
========

Release types
-------------

We provide different releases and apply security updates on a regular basis.

Standard version
----------------

If you don't select a certain version, our default will be used. We decided to
default to the following version:

.. code-block:: bash

  [isabell@stardust ~]$ uberspace tools version show postgresql
  Using 'postgresql' version: 15
  [isabell@stardust ~]$

Show available versions
-----------------------

Use ``uberspace tools version list postgresql`` to show all selectable versions:

.. code-block:: bash

  [isabell@stardust ~]$ uberspace tools version list postgresql
  - 12
  - 13
  - 14
  - 15
  [isabell@stardust ~]$

Change version
--------------

You can select the version using ``uberspace tools version use postgresql <version>``:

.. code-block:: bash

  [isabell@stardust ~]$ uberspace tools version use postgresql 12
  Selected postgresql version 12
  The new configuration is adapted immediately. Minor updates will be applied automatically.
  [isabell@stardust ~]$

Update policy
-------------

We update all versions on a regular basis. Once the `support <https://www.postgresql.org/support/versioning/>`_ ends, the branch reaches its end of life (EOL), is no longer supported and will be removed from our servers.

+--------+-------------------------+------------------+
| Branch | State                   | Supported Until  |
+========+=========================+==================+
| 12     | Active                  | November 2024    |
+--------+-------------------------+------------------+
| 13     | Active                  | November 2025    |
+--------+-------------------------+------------------+
| 14     | Active                  | November 2026    |
+--------+-------------------------+------------------+
| 15     | Active                  | November 2027    |
+--------+-------------------------+------------------+
