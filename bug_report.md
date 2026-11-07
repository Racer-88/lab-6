
# Lab 06 Bug Report

| Bug | Test(s) that failed |
| --- | --- |
| 1. POST returns incorrect status code | `test_create_artwork`; `created_artwork` fixture caused errors in 6 dependent tests |
| 2. Duplicate check is case-sensitive | `test_create_duplicate_ignores_case` |
| 3. Artwork counts as a duplicate of itself | `test_update_same_title_and_artist_is_allowed` |
| 4. DELETE does not actually delete | `test_delete_artwork` |
| 5. Artist filter only matches the start of a name | `test_filter_by_artist[lowercase-partial]` |
