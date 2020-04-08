# Gaining Traction

> Models and Attributes

- User
    - Username
    - Email
    - Password
---
- Goal 
    - Title
    - Description
    - Start Date (created_at column from table?)
    - Current Progress (sums time spent on all tasks together and displays progress towards reaching 10,000 hours)
    - Complete (boolean? and maybe use updated_at column from table for reference to date completed?)
---
- Task
    - Title
    - Description
    - Time Spent On Task
---
> Associations
 - User
    - has_many :goals
    - has_many :tasks, through: :goals
---
- Goal
    - belongs_to :user
    - has_many :tasks

---
- Task
    - belongs_to :goal
    - belongs_to :user
---

