| Short Name           | Full Name                 | Type   | Length | Constraint | Example                              |
| -------------------- | ------------------------- | ------ | ------ | ---------- | ------------------------------------ |
| mentor_id            | ID of the mentor          | AN     | 36     | Required   | 3fa85f64-5717-4562-b3fc-2c963f66afa6 |
| mentor_firstname     | First name of the mentor  | A      | 50     | Required   | Alice                                |
| mentor_lastname      | Last name of the mentor   | A      | 50     | Required   | Smith                                |
| mentor_description   | Description of the mentor | TEXT   | -      | Required   | Senior backend developer             |
| mentor_expertise     | Mentor's expertise        | TEXT[] | -      | Required   | ["JavaScript", "Node.js"]            |
| mentor_disponibility | Mentor's availability     | AN     | 100    | Required   | Mondays 2-5 PM, Fridays 10-12 AM     |

| Short Name           | Full Name                 | Type | Length | Constraint | Example                              |
| -------------------- | ------------------------- | ---- | ------ | ---------- | ------------------------------------ |
| mentee_id            | ID of the mentee          | AN   | 36     | Required   | 9d2a42e1-7623-4c3b-b3a6-1a2c00e5461e |
| mentee_firstname     | First name of the mentee  | A    | 50     | Required   | John                                 |
| mentee_lastname      | Last name of the mentee   | A    | 50     | Required   | Doe                                  |
| mentee_description   | Description of the mentee | TEXT | -      | Required   | Junior frontend developer            |
| mentee_cursus        | Mentee's cursus           | A    | 100    | Required   | Web development bootcamp 2024        |
| mentee_disponibility | Mentee's availability     | A    | 100    | Required   | Evenings and weekends                |
| mentee_objective     | Mentee's objective        | TEXT | -      | Required   | Improve JavaScript and React skills  |

| Short Name        | Full Name             | Type | Length | Constraint | Example                              |
| ----------------- | --------------------- | ---- | ------ | ---------- | ------------------------------------ |
| session_id        | ID of the session     | UUID | 36     | Required   | 1b5cf9e0-3d74-4e67-aaa9-8a4e7a1b2243 |
| session_date      | Date of the session   | DT   | -      | Required   | 2025-05-26                           |
| session_status    | Status of the session | A    | 20     | Required   | planned or completed or canceled     |
| session_objective | Objective of session  | TEXT | -      | Required   | Review mentee's portfolio            |
| session_guest     | Guest of the session  | A    | 100    | Required   | CTO of Partner Company               |
| session_report    | Session report        | TEXT | -      | Required   | Discussed roadmap and progress       |

| Short Name         | Full Name          | Type | Length | Constraint          | Example                              |
| ------------------ | ------------------ | ---- | ------ | ------------------- | ------------------------------------ |
| feedback_id        | ID of the feedback | AN   | 36     | Required            | 6fd1c298-812f-4b6c-918c-eaa21d6b5f6f |
| feedback_rating    | Rating             | N    | -      | Required, Check 1-5 | 4                                    |
| feedback_comment   | Feedback comment   | TEXT | -      | Optional            | Very helpful session                 |
| feedback_createdAt | Date of feedback   | DT   | -      | Required            | 2025-05-26T14:30:00Z                 |

| Short Name          | Full Name              | Type | Length | Constraint      | Example                              |
| ------------------- | ---------------------- | ---- | ------ | --------------- | ------------------------------------ |
| notification_id     | ID of the notification | AN   | 36     | Required        | 2dc3bff1-1c90-4a3c-9cf3-41c9aee6e0cf |
| notification_text   | Notification message   | TEXT | -      | Required        | You have a new session scheduled     |
| notification_date   | Notification date      | DT   | -      | Required        | 2025-05-25T18:00:00Z                 |
| notification_status | Notification status    | TEXT | -      | Required, Check | unread or read                       |
| notification_type   | Notification type      | TEXT | -      | Required, Check | reminder or information or alert     |

_légende_ :

**A** = Alphabetic

**N** = Numeric

**AN** = Alphanumeric (souvent utilisé pour UUID ou identifiants)

**DT** = DateTime/TimeStampTZ

**TEXT / TEXT[]** = chaînes longues ou tableaux
