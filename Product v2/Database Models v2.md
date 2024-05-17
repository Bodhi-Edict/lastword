---
Date Created: 2024-05-14
---
### Done

User
- Email
- EmailVerified
- HashedPassword
- Avatar

Session
- UserId
- ExpiresAt

EmailVerification
- UserId
- Email
- Code
- ExpiresAt

PasswordResetTokens
- UserId
- ExpiresAt

Class
- Name
- Subject
- Description
- SubjectId

Subject
- Text

ClassMember
- ClassId
- User Id
- Code
- Type - Teacher or Student

Assignment
- Name
- Due Date
- Max Score
- Time Limit
- ImageUrl
- AssignmentTemplateId
- ClassId
- isLive
- isSample
- ShowConceptHints

AssignmentTemplate
- Title
- Image Url
- AssistantId
- ConceptGraph
- Prompt (if needed)

### To Do

Concept
- QuestionText
- AssignmentTemplateId
- Position

ConceptExplanationText
- ConceptId
- AlternateText
- Embedding Vector

Attempt
- UserId
- AssignmentId
- Score
- FinalExplanationId
- SubmittedAt 

Explanation
- Text
- Embedding -> Can choose to not store
- CorrectConcepts
- UserId
- AttemptId

Answer
- ExplanationId
- QuestionId
- ComputedAnswer
- IsCorrect -> Computed property 
- Explanation text

Questions
- Text
- Answer
- ConceptSubGraph
- AssignmentTemplateId

Question - Assignment Template
- QuestionId
- AssignmentTemplateId
