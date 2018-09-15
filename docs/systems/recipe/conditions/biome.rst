Biome
=====

Break Down:
-----------

The Biome condition allows for the recipe to either happen in a specific biome, or outside said biome. It has two fields,
one required: biome, which is the name, and one optional: inBiome, which defaults to true, and determines whether the
recipe needs to be in, or outside of the biome.

Example:
--------

.. code-block:: json

    {
        "type": "base:biome",
        "biome": "minecraft:plains",
        "inBiome": true
    }