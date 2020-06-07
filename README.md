# wizard_app DB設計
## usersテーブル
|Column|Type|Options|
|------|----|-------|
|name|text|null: false|
|age|integer|null: false|
|email|string|null: false|
|password|string|null: false|
### Association
- has_one :address

## addressesテーブル
|Column|Type|Options|
|------|----|-------|
|zipcode|integer||
|address|text||
|user_id|reference|optional: true|

### Association
- belongs_to :user
