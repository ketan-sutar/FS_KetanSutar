# FS_KetanSutar 


# Student Commute Optimizer (Full Stack) – Solution

Problem Definition:- 
- Students often travel from home → college individually. This increases cost, traffic, and pollution.
- The Student Commute Optimizer provides a safe, anonymous, and efficient carpool/ride-sharing platform to connect students traveling along similar routes.

Solution:-
# 1. Frontend:
-- The frontend should:
⋅⋅⋅⋅* Take home → destination input
⋅⋅⋅⋅* Show nearby students on overlapping routes
⋅⋅⋅⋅* Keep users anonymous
⋅⋅⋅⋅* Allow private chat

## Components or Core Feature: 

Map UI: Enter home → destination; display route (polyline) using Google Maps or Leaflet. Optimize with tile rendering & simplified polylines.

Nearby Students: Show icons for overlapping routes; clickable to open chat.

Anonymous Profiles: Each student gets a UUID-based username (Rider_XXXX); no real names or emails.

Chat: Real-time private chat via WebSocket (Socket.IO) or Firebase.

Authentication: Minimal – generate UUID Rider ID, no password required.

Performance: Use clustering & reduce polyline points for smooth map rendering.






2. Backend:

## System Architecture Diagram
You can view the frontend and backend architecture diagram here:  
[Frontend + Backend System Architecture](https://app.eraser.io/workspace/BFYdl3jsqCY9F6aoewba?elements=cwBo9byY9_j93arIh3eMHA)

