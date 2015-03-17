==========
``config``
==========

.. autoclass:: invoke.config.Config
    :members:
    :special-members:
    :exclude-members: __weakref__

    .. py:attribute:: _defaults

        Default configuration values, typically hardcoded in the
        CLI/execution machinery.

    .. py:attribute:: _collection

        Collection-driven config data, gathered from the collection tree
        containing the currently executing task.

    .. py:attribute:: _system_path

        Path to loaded system config file, if any.

    .. py:attribute:: _system_found

        Whether the system config file has been loaded or not (or ``None``
        if no loading has been attempted yet.)

    .. py:attribute:: _system

        Data loaded from the system config file.

    .. py:attribute:: _user_path

        Path to loaded user config file, if any.

    .. py:attribute:: _user_found

        Whether the user config file has been loaded or not (or ``None``
        if no loading has been attempted yet.)

    .. py:attribute:: _user

        Data loaded from the per-user config file.

    .. py:attribute:: _project_home

        Parent directory of the current root tasks file, if applicable.

    .. py:attribute:: _project_path

        Path to loaded per-project config file, if any.

    .. py:attribute:: _project_found

        Whether the project config file has been loaded or not (or ``None``
        if no loading has been attempted yet.)

    .. py:attribute:: _project

        Data loaded from the per-project config file.

    .. py:attribute:: _env

        Config data loaded from the shell environment.

    .. py:attribute:: _runtime_path

        Path to the user-specified runtime config file.

    .. py:attribute:: _runtime

        Data loaded from the runtime config file.

    .. py:attribute:: _runtime_found

        Whether the runtime config file has been loaded or not (or ``None``
        if no loading has been attempted yet.)

    .. py:attribute:: _overrides

        Overrides - highest possible config level. Typically filled in from
        command-line flags.
