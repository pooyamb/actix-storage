## Version 0.2-alpha.3
- Restructured the code
- Bug fixes

## Version 0.2-alpha.2
- Updated to actix-storage 0.2-alpha.2
- There is now a new feature flag `v01-compat` for backward compatiblity with 0.1 global scopes

## Version 0.2-alpha.1
- Updated to actix-storage 0.2 with support for scopes based on sled's trees
- **Backward incompatibility:** Global scope is now a subtree of the main sled's db, so you'll need to migrate your data from sled's global tree to actix-storage's global tree on `STORAGE_GLOBAL_SCOPE` exported as a constant from `actix-storage::GLOBAL_SCOPE`
