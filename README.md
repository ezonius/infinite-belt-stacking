# Infinite Belt Stacking

Reach for the skies! Adds a postgame **infinite technology** with endless tiers of belt stacking
(transport-belt-capacity-3, `max_level = infinite`). Requires a mod that adds stack inserters, such as the
Space Age DLC or the Stack Inserters mod — the mod **crashes with a readable error** at load time if neither
is present.

## Features

- Raises `max_belt_stack_size` (via `utility-constants`) to 250 ("infinity, rounded down") for all
  loaders and stack inserters that already support stacking.
- Adds the infinite technology **Belt capacity 3**, which grants `belt-stack-size-bonus` and
  `bulk-inserter-capacity-bonus` per level.
  - Prerequisites: `transport-belt-capacity-2` and `inserter-capacity-bonus-7`.
  - Cost formula: `1.1^(L-3)*1000+3000`, 120s per level, all science packs (plus agricultural science
    with Space Age).

## Settings

| Setting | Type | Default | Description |
| --- | --- | --- | --- |
| Inserter hand stack max sprites | startup, int | 250 | Maximum number of item sprites an inserter hand draws while holding a stack. Lower values improve performance at the cost of visuals; cannot exceed the max belt stack size. |

## Compatibility

- Factorio **2.1**. Works with or without the Space Age DLC (requires *some* stack inserter source:
  `space-age` or `stack-inserters`).

## License

MIT — see [LICENSE](LICENSE).
