# Attributes

Attributes are stats that an entity can have, such as health, strength, charisma, speed, etc. They all have a name, a
short name, a base value, and can optionally have a modifier.
The short name is used as a reference for the attribute.

## Modifier

An attribute modifier is an optional [expression](expressions.md) that is used in games like Dungeons & Dragons or other
d20-based systems.
When providing the `modifier`, the variable `entity` will be available, as well
as [value references](expressions.md#value-references) to the rest of the definition.
