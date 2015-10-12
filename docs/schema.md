# Schema Information

## workspace
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
name        | string    | not null
address     | string    | not null
overall     | integer   | not null
wifi        | integer   | not null
power       | integer   | not null
seating     | integer   | not null
pricing     | integer   | not null
hours       | text      | not null


## reviews
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
user_id     | integer   | not null, foreign key (references users), indexed
workspace_id| integer   | not null, foreign key (references workspace), indexed
body        | text      |
overall     | integer   | not null
wifi        | integer   |
power       | integer   |
seating     | integer   |
pricing     | integer   |


## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
email           | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique
first_name      | string    | not null
last_name       | string    | not null
location        | string    | not null

*** Additional Note: ***
Planning to use the Paperclip gem for a user's profile pic and workspace's profile pic
and pictures uploaded by registered users.
