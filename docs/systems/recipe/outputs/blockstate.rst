BlockState
==========

Break Down:
-----------

The Blockstate output is comprised of three section, one required: blockState, and two optional: offset, and tileEntityNBT.

The blockstate has one required field: block which must match a valid block, and then one optional field:
properties which is an object contain the properties that should be set. (Note that missing properties will be treated
as default.)

The offset is optional, and all three of it's fields (x, y, and z) are all optionals and default to zero, this offset is
a location different from the block that is handling the current recipe.

The tileEntityNBT is optional, and will be used to set NBT such as an ItemBlock would.

Example:
--------

.. code:: json

    {
        "type": "base:blockstate",
        "blockState": {
            "block": "minecraft:chest",
            "properties": {
                "facing": "north"
            }
        },
        "offset": {
            "x": 0,
            "y": 1,
            "z": 0
        },
        "tileEntityNBT": {
            "LootTable": "minecraft:simple_dungeon"
        }
    }