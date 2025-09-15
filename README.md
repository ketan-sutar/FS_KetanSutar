# FS_KetanSutar 


# Student Commute Optimizer (Full Stack) – Solution

Problem Definition:- 
- Students often travel from home → college individually. This increases cost, traffic, and pollution.
- The Student Commute Optimizer provides a safe, anonymous, and efficient carpool/ride-sharing platform to connect students traveling along similar routes.

Solution:-
# 1. Frontend:
Frontend (React – Student Facing)

Map UI: Enter home + school → draw route (Google Maps API / Leaflet + OpenStreetMap)

Nearby Students: Display icons of overlapping routes

Anonymous Profiles: Shown as Rider_1234

Chat Integration: Click student icon → chat window opens

Authentication: Minimal – generate UUID Rider ID, no password required.

Performance: Use clustering & reduce polyline points for smooth map rendering.








2. Backend:
   The backend handles:

Comparing student routes to find overlaps.

Suggesting ride-sharing matches.

Ensuring anonymity of students.

Providing real-time chat for matched students.

Goal: Efficient, scalable, and secure backend without revealing identities.



#Approach:


1- API Design


2- Anonymization Service


3- Chat Service
4- Database Design
5- Route Matching







#### System Architecture Diagram

![Frontend + Backend Architecture](https://github.com/user-attachments/assets/7dcac3c6-696c-43d8-bb4a-9647a2fa4b61)

You can also view it interactively on Erase.io:  
[Frontend + Backend Architecture Diagram](https://app.eraser.io/workspace/BFYdl3jsqCY9F6aoewba?elements=cwBo9byY9_j93arIh3eMHA)
