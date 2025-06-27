### sanakirja-org CHANGELOG

---

<details id="v1.1.0">
    <summary>v1.1.0</summary>
    
    - Added the `gender` field to the result dictionary, which displays the linguistic gender as a `str` type, or None, if not applicable.
    - Added the URL to all applicable entries in the form of a `word_url` key, or `category_url` in the case of the `categories` field.
        - In the case of the `definitions` field, the applicable words and their URLs were added under a new `words` key, which is a list of `dict` types.

    - Changed the types of the `multiple_spellings`, `relations` and `categories` fields to a list of `dict` types from a list of `str` types.
    - Changed the type of the `additional_source_languages` field to a `dict` type from a list of `str` types.
    - Changed the type of the `inflections` field to a list of `dict` types from a `dict` type.
        - The inflection type is now a value of the `type` key instead of being a key itself.
    - Changed the entries of the `suggestions` field (akin to old `similar_words`) to be ordered based on the font sizes of the words.

    - Fixed target language key appearing in the `translations` field, when no translations were found.
    
    - Removed graceful exiting from the CLI tool, to assist with debugging.

    - Replaced the `similar_words` field with the fields `did_you_mean`, `suggestions` and `found_examples`.
        - First of these is a `dict` type, while the two latter ones are lists of `dict` types.
</details>
<details id="v1.0.0.post1">
    <summary>v1.0.0.post1</summary>
    
    - Updated licensing.
</details>
<details id="v1.0.0">
    <summary>v1.0.0</summary>
    
    - Initial release.
</details>