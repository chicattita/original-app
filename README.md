# README
## userテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| id(PK)             | integer | null: false               |
| name               | string  | null: false               |
| nickname           | string  | null: false               |
| email              | string  | null: false, unique: true |
| encrypted_password | string  | null: false               |
| date_of_birth      | date    | null: false               |


### Association
- has_many :comments
- has_many :conducts


## conductsテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |


### Association


## commentsテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |


### Association






