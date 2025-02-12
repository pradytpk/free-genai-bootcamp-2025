## Business Requirements

We are building a learning portal that acts as launchpad for study activities put also lets browse our vocabulary library

- have an inventory of words in the target language
- have a group os words to thematic categories(e.g)
- we want to sore study sessions eg word right and wrong

### API end Points

#### `GET /api/words`

    - return a list of words 100 words at a time
    - pagination

##### Response Json

```json
[
    {
        "id": 1,
        "kanji": "人”,
        "romaji": "jin",
        "english": "persion",
        "group_id": 1,
    }
]
```

- `GET /api/words/:id`

- `GET /api/groups`
- `GET /api/groups/:id`

- `GET /api/study_sessions`
