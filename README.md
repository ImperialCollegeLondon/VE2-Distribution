# Virtual Experience Engine Distributables

Welcome to the **Virtual Experience Engine (VE2)** Tooling Guide!  
This document provides a high-level, non-exhaustive overview for setting up and using VE2 in your Unity projects.

The VE2 tools, the installer, and this setup guide are all in Alpha, and are a work in progress.

---

## Installation Guide

1. **Create a Unity Project**  
   - Set up a new **URP** (Universal Render Pipeline) Unity project on **Unity version 6.0.44**.

2. **Install VE2 Package**  
   - Open the **Package Manager**.
   - Click on **Install Package from Git URL**.
   - Paste the following URL:  
     `git+https://github.com/ImperialCollegeLondon/VE2-Distribution.git?path=VE2Installer#main`

3. **Install VE2**  
   - In Unity's top menu bar, navigate to **VE2 > Install VE2**.

4. **Configure XR Settings**  
   - Open **Unity’s Project Settings**.
   - Go to **XR Plug-In Management** and ensure **OpenXR** is enabled.

5. **Set Up XR Plugin**  
   - Navigate to **XR Plug-In Management > OpenXR**.
   - Under **Enabled Interaction Profiles**, add **Oculus Touch Interaction Profile**.

6. **Set Up Your Scene**  
   - Create a new scene in Unity.
   - Go to **VE2 > Setup Scene**.

7. **Start Local Server**  
   - In the top-right corner, click on **VE2: Start Local Server**.

8. **Play the Scene**  
   - Enter **Play Mode** and begin interacting with VE2!

---

## Known Issues

- **Grabbables:**  
   If you join a session where a grabbable object has already been grabbed and dropped, and then pick it up and drop it again, the grab/drop action is overridden.

- **Kinematic RBSyncables:**  
   Kinematic RBSyncables may travel further than expected when dropped.

- **Pressure Plate Configuration:**  
   Some inspector settings on the Pressure Plate component, such as tooltips and haptics, shouldn't be present.

---

## Console Warnings You Can Ignore

- **Installation Warnings:**  
   You may see warnings like:  
   `"Asset Packages/com.ic.ve2installer/package.json has no meta file, but it's in an immutable folder. The asset will be ignored."`

- **DoTween Modules:**  
   Errors related to DoTween modules may appear, but the functionality is unaffected.

- **VComponents Inspectors:**  
   Inspectors for VComponents may spam the console with “invalid layout data” warnings. These can be ignored, though they can be a nuisance.

- **VR Package Warnings:**  
   VR-related packages may output irrelevant console messages. Feel free to ignore them.

- **Inactive GameObject Coroutine Warning:**  
   The warning:  
   `"Coroutine couldn't be started because the game object 'vrPlayer' is inactive!"`  
   is harmless and can be ignored.

---

## Features Not Yet Implemented

- **Infopoints**  
- **Reset VR Neutral Position**  
- **Inspector Configurations** for various VComponents  
- **Instancing Configuration** (max number of players, etc.)  
- **Voice Chat Configuration**  
- **World Build System** (still placeholder)  
- **Auto Configuration** for XR packages, interaction profiles, etc.  
- **Build Features** that won’t affect plugin developers

---

## Use-Cases Not Yet Investigated

- **Teleporting Networked Rigidbodies**  
- **Using Non-VE2 Players**  
- **Changing Player Avatars**  
- **Modifying Scene Settings** (physics settings, etc.)

---

## Copyright Notice

**Virtual Experience Engine (VE2)**  
Copyright © [2025] **Imperial College London**  

All rights reserved.  

This software and its associated files are proprietary to **Imperial College London**.  
Unauthorized copying, distribution, or sharing of this code, in whole or in part,  
to individuals or entities outside of Imperial College London is strictly prohibited  
without prior written permission.  

This software is provided exclusively for use within Imperial College London  
and may only be accessed, modified, or utilized by authorized personnel or  
approved collaborators.  

For inquiries regarding permissions, please contact:  
[ftoveyan@ic.ac.uk](mailto:ftoveyan@ic.ac.uk)
