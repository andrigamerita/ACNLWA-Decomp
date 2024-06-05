# Game Reversing Notes

## Items

`romfs/Item/Param/Item.bin` contains properties about the functional nature of items. The table contains 30-byte entries ordered by item id, and starts with item 2000, for a total of 5932 entries. Meaning of colums is not always clear, and changes with context. Items that are of a similar category have textually similar bytes for some columns.

0. Could indicate some kind of item variant (eg, this starts at 01 and ends at 6C for bells).

...

27. Common flags of some kind. Most items are 02, and items marked 06 are eatable.

...

All strings for filename of 3d models or textures for items seem to be in the game executable, however they follow an unique order based more on functionality of items rather than aestetic categorization. (For example, while furniture items are ordered by sets in the item id database, these strings might be ordered for all items of a kind, and not necessarily following a relative id ordering; for example, names of 3d model files for lamps appear to be listed one after another in the executable, even if many are of different sets.)

