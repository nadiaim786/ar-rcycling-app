# ar-recycling-app
AI-Based AR Waste Detection & Recycling Guidance System (Unity AR Foundation)

🧩 CORE COMPONENTS (UNITY SETUP)
🟢 1. AR SESSION (World Tracking Controller)

Unity AR Foundation component

Role:
Starts AR tracking
Connects to ARCore on phone
Initializes camera + sensors
🟢 2. XR ORIGIN (AR RIG)
Contains:
AR Camera (Main Camera)
Device tracking space
Role:
Moves virtual world based on phone movement
Acts as AR coordinate system
🟢 3. AR CAMERA
Components:
Camera
AR Camera Manager
AR Camera Background
Tracked Pose Driver
Role:
Shows real-world live camera feed
Aligns virtual objects with real world
🟢 4. AR PLANE MANAGER
Role:
Detects flat surfaces (floor, table)
Generates AR planes in real time
🟢 5. AR RAYCAST MANAGER
Role:
Detects where user taps on real surfaces
Converts screen touch → real-world position
🟢 6. PLACEMENT SCRIPT (YOUR SCRIPT)

Example: PlaceObjectOnPlane.cs

Role:
Spawns object (cube / recycle icon) on detected plane
Handles tap interaction
