Captivote
=========

## Question
### question_id
### question_text_or_img: string
### author: email
### timer: NUL | # of seconds

### Example: 
Q: Mirror mirror on the wall, who's the fairest of them all?
A0: Me
A1: <text from user 0>
A2: <text from user 1>
A3: ...

---

## Answer
### answer_id
### parent: question_id
### answer_text_or_img: string

---

## Vote
### vote_id
### type: (answer_id | question_id)
### parent: question_id
### up_votes: int
### down_votes: int

---

## Votee
### votee_id
### user: email
### vote: int
### parent: vote_id

---

## User
### email: string
### password: hashed string
### alias: string

---

## Group
### name
### description
### user_limit: int | NUL
### Example
- AEPi has 3 games running

---

## Score
### group_id
### email: string
### votes: int
