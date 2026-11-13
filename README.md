# WaveCymatix-Visuals

Curated projectM presets, textures, and sprites for WaveCymatix. Assets are kept together rather than split by operating system or performance tier; the catalog records their inventory and assessment state.

## Catalog

[`catalog.json`](./catalog.json) lists every asset using repository-relative paths with `/` separators. Presets currently have no performance classification: their `minimumTierLevel` is `null` and their assessment status is `pending`.

Tier levels use the names already used by the WaveCymatix installers:

| Name | Level |
| --- | ---: |
| `very_low` | 0 |
| `low` | 1 |
| `medium` | 2 |
| `high` | 3 |

Once assessed, a preset is eligible when its minimum tier level is less than or equal to the detected machine tier. Thus, a `high` machine includes presets classified for all four levels, along with their required visual resources.

Preset-to-resource dependency mapping and performance assessment are still pending. No installer currently consumes this catalog.

## Asset inventory

- `presets/` — curated `.milk` presets
- `textures/` — texture images
- `sprites/` — sprite images

Asset attribution and licensing have not yet been reviewed as part of this initial catalog.
