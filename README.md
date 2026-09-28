# clabbers-lexicons

Dictionary files that the Clabbers apps (desktop, Android and iOS) download when a player asks for
them in Settings > Lexicons. Nothing else lives here.

Each file is encrypted, in the same form the app installers already carry, and opens only inside
the app. Before using a file the app checks its size and SHA-256 fingerprint against the values
pinned in its own code, and refuses any file that does not match.

## Release `lexicons-2026-09-29`

| File | Lexicon | Used by | Bytes | SHA-256 |
|---|---|---|---|---|
| `csw24-desktop.db` | CSW24 (Collins Scrabble Words 2024) | desktop | 58,929,152 | `413929b57a8fbdeb15772cb048f4d12da27d19f8cf32cf49aef4d867cf075fc8` |
| `csw24-mobile.db` | CSW24 (Collins Scrabble Words 2024) | phones | 58,929,152 | `3f4a96496178ad54e750459216910474090263f2b95940711746869cf6a6d18f` |
| `nwl2023-desktop.db` | NWL2023 (NASPA Word List 2023) | desktop | 42,467,328 | `c34a4b65803a50656855d5f32df2b140669e934cb01d56f7af494263bc8cb453` |
| `nwl2023-mobile.db` | NWL2023 (NASPA Word List 2023) | phones | 42,467,328 | `12de1b008854ce938460187f714403dc0f3cc4b7c33da0e3bf082bc08a23645e` |

A new release is published only together with an app update that pins its fingerprints; files
are never replaced in place.
