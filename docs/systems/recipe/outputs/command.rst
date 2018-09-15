Command
=======

Breakdown
---------
Command output takes a singe required parameter: command, which is a string that will be run by minecraft. Note: This is
similar to having the command run from a Command Block, rather than by a player

Example
-------

.. code-block:: json

    {
        "type": "base:command",
        "command": "xp set @p 0 levels"
    }