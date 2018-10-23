BlockState
==========

Break Down:
-----------

The Blockstate input is comprised of two section, one required: blockState, and one optional: offset.

The blockstate has one required field: block which must match a valid block, and then one optional field:
properties which is an object containing valid blockstate properties. (Note that missing properties will be considered
as all properties matching.)

The offset is optional, and all three of it's fields (x, y, and z) are all optionals and default to zero, this offset is
a location different from the block that is handling the current recipe

Example:
--------

.. code:: json

    {
        "type": "base:blockstate",
        "blockState": {
            "block": "minecraft:stone",
            "properties": {
                "variant": [
                    "granite"
                ]
            }
        },
        "offset": {
            "x": 0,
            "y": 1,
            "z": 0
        }
    }
