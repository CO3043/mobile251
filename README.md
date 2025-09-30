# Lost and Found app
An application to support students at Ho Chi Minh City University of Technology (HCMUT) in finding and returning lost items quickly and anonymously.

## Motivation của project: 
At HCMUT, students frequently lose personal belongings in classrooms, libraries, or campus areas.
Currently, lost items are typically handed to building guards or posted on Facebook groups. Both approaches have major issues:
+ Guard-dependent: not always available, limited working hours, students must physically check multiple desks.
+ Facebook posts: scattered across multiple groups (K22, K23, CNCP, etc.), posts quickly get buried, no anonymity in messaging.

## Our solution provides:
- A centralized lost-and-found system for the university.
- Anonymous posting & messaging via alias usernames.
- Thread-based posts per building → less noise, easier search.
- Verification flow for claims → reduces scams.
- Audit logs & reporting for security.

## Functional Requirement:
- Sign up with HCMUT email + OTP (15 min).
- Anonymous alias usernames (e.g., User#1234).
- Post items with building, floor, time, description, images.
- Follow threads & get push notifications (<30s).
- Claim items with proof; post owner can accept/reject.
- Report posts/claims (spam, fraud, misconduct).
- Admin: view posts, claims, logs, filter by building/status.

## Non-functional Requirements:
- Uptime ≥ 90%.
- API list posts ≤ 500ms (95%, <1000 posts).
- Push notifications ≤ 30s.
- Emails encrypted, only alias is public.

## Scope:
- Now: Campus 2 only.
- Future: Campus 1, integration with security office, lost-item analytics.
