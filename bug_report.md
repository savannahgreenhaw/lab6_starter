# Bug Report

|               Bug                               | Test(s) that failed |

| POST returns 200 instead of 201 | |
| Duplicate check is case-sensitive | |
| Artwork is considered a duplicate of itself | |
| DELETE does not remove artwork | |
| Artist filter only matches prefixes | |


##### 1
BUG: POST returns 200 instead of 201 
FAILED TESTS: 
test_create_artwork, test_create_artwork_is_saved, test_update_artwork, test_delete_artwork, test_create_duplicate, test_create_duplicate_ignores_case, test_update_same_title_and_artist_is_allowed

##### 2
BUG: Duplicate check is case-sensitive
FAILED TEST: test_create_duplicate_ignores_case

##### 3
BUG: Artwork is considered a duplicate of itself
FAILED TEST: test_update_same_title_and_artist_is_allowed


##### 4
BUG: DELETE does not remove artwork
FAILED TEST: test_delete_artwork


##### 5
BUG: Artist filter only matches prefixes
FAILED TESTS: test_filter_by_artist[monet-expected_titles1]


