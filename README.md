# README
## userテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| id(PK)             | integer | null: false               |
| username           | string  | null: false               |
| email              | string  | null: false, unique: true |
| encrypted_password | string  | null: false               |
| date_of_birth      | date    | null: false               |
| birth_place        |         | null: false               |

### Association
- has_many :comments
- has_many :conducts
- has_many :status


## conductsテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| id                 |
| user_id            |
| content_name       |
| content            |

### Association
- has_many :comments
- belongs_to :user
- belongs_to :statu


## commentsテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| id                 |
| user_id            |
| conduct_id         |
| content            |

### Association
- belongs_to :user
- belongs_to :conduct


## statusテーブル
| Column             | Type    | Option                    |
|-                   |-        |-                          |
| user_id            |
| conduct_id         |

### Association
- has_many :conducts
- belongs_to :user




