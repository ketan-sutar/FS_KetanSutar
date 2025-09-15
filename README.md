# FS_KetanSutar

## Student Commute Optimizer (Full Stack) – Solution

### Problem Definition
- Students often travel from home → college individually, which increases cost, traffic, and pollution.  
- The **Student Commute Optimizer** provides a **safe, anonymous, and efficient carpool/ride-sharing platform** to connect students traveling along similar routes.

---

## Solution

### 1. Frontend
**Technology:** React – Student Facing  

**Features:**
- **Map UI:** Enter home + school → draw route (Google Maps API / Leaflet + OpenStreetMap)  
- **Nearby Students:** Display icons of overlapping routes  
- **Anonymous Profiles:** Shown as `Rider_1234`  
- **Chat Integration:** Click student icon → chat window opens  
- **Authentication:** Minimal – generate UUID Rider ID, no password required  
- **Performance:** Use clustering & reduce polyline points for smooth map rendering  

**Frontend Approach / Links:**
1. **Student Login / UUID Generation**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Student%20Login%20and%20UUID%20Generation)

2. **Enter Route (Home → Destination)**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Enter%20Route)

3. **Map Rendering & Nearby Students Display**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Map%20Rendering%20%26%20Nearby%20Students%20Display)

4. **Clicking a Student Icon → Open Chat**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Clicking%20a%20Student%20Icon%20%E2%86%92%20Open%20Chat)

---

### 2. Backend
The backend handles:  
- Comparing student routes to find overlaps  
- Suggesting ride-sharing matches  
- Ensuring anonymity of students  
- Providing real-time chat for matched students  

**Goal:** Efficient, scalable, and secure backend without revealing identities.

**Backend Approach / Links:**
1. **API Design**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/API%20Design)

2. **Anonymization Service**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Anonymization%20Service)

3. **Chat Service**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Chat%20Service)

4. **Database Design**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Database%20Design)

5. **Route Matching**  
   [Link](https://github.com/ketan-sutar/FS_KetanSutar/blob/main/Route%20Matching)

---
## Technology Stack

| Layer          | Technology                                         | Purpose                                                   |
| -------------- | -------------------------------------------------- | --------------------------------------------------------- |
| **Frontend**   | React.js                                           | Component-based UI, fast rendering                        |
| **Styling**    | Tailwind CSS                                       | Clean, responsive design                                  |
| **Maps & Routing** | Google Maps API / Leaflet + OpenStreetMap       | Route drawing & nearby student visualization              |
| **Backend**    | Node.js / FastAPI                                  | API endpoints, route matching, chat handling              |
| **Realtime Chat** | Firebase Realtime DB / WebSocket (Socket.IO)    | Real-time messaging between anonymous users               |
| **Database**   | MongoDB / PostGIS                                  | User, route, and chat data storage; Geo-spatial queries   |
| **Authentication** | UUID Generator                                 | Anonymous login / unique Rider IDs                        |
| **Deployment** | Vercel / Netlify (frontend), Heroku / Render (backend) | Hosting frontend and backend services                 |


---
### System Architecture Diagram

![Frontend + Backend Architecture](https://github.com/user-attachments/assets/7dcac3c6-696c-43d8-bb4a-9647a2fa4b61)

You can also view it interactively on Erase.io:  
[Frontend + Backend Architecture Diagram](https://app.eraser.io/workspace/BFYdl3jsqCY9F6aoewba?elements=cwBo9byY9_j93arIh3eMHA)
