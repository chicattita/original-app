# README
## userテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| name               | string  | null: false               |
| nickname           | string  | null: false               |
| email              | string  | null: false, unique: true |
| encrypted_password | string  | null: false               |
| id(PK)             | integer | null: false               |
| date_of_birth      | date    | null: false               |


### Association
- has_many :comments
- has_many :conducts



## commentテーブル
### Association



## comment_usersテーブル
### Association



## conductテーブル
### Association