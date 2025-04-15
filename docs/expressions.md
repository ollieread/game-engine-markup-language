# Expressions

Expressions are ways to provide values, whether constant, variables or calculated.

## Values

Expressions can contain two value types:

- Constant values - `const`
- Variable values - `var`

Constant values are values that are fixed and do not change, and will always be whole numbers (integers).

Variable values are values that can change, and the particular schema definition making use of the expression will have
in its documentation the variables that are available.

### Value References

You can also reference the current definition using JSON pointers that are _always_ relative to the root of the
definition, and start with a `$`.
If you wish to use the value as part of another variable, you must surround it with `{` and `}`.
For example, when defining the `modifier` of an [attribute](attributes.md),
you can access the entity attribute like so:

```
entity.attributes.{$shortName}.calculatedValue
```

Which in the case of say `Strength` that has a short name of `STR` would be:

```
entity.attributes.STR.calculatedValue
```

## Operators

TBW
