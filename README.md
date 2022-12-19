#usersテーブル

|Column              | Type   | Options     |
|--------------------| -------| ------------|
|email               | string | null: false |
|encrypted_password  | string | null: not |
|name                | string | null: not |
|profile             | text   | null: not |
|occupation          | text   | null: not |
|position            | text   | null: not |


#commentsテーブル
| Column     | Type       | Options                        |
| ------     | ---------- | ------------------------------ |
| content    | text       | null: not                      |
| prototype  | references | null: not, foreign_key: true   |
| user       | references | null: not, foreign_key: true   |

#prototypesテーブル
| Column      | Type       | Options                        |
| ------------| ---------- | ------------------------------ |
| title       | string     | null:not                       |
| catch_copy  | text       | null:not                       |
|concept      | text       | null:not                       |
|user         | references | null: not, foreign_key: true   |

