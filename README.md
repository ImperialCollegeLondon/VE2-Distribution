# Virtual Experience Engine Distributables

Welcome to the **Virtual Experience Engine (VE2)** Tooling Guide!  
This document provides a high-level, non-exhaustive overview for setting up and using VE2 in your Unity projects.

The VE2 tools, the installer, and this setup guide are all in Alpha, and are a work in progress.

---

## Installation Guide

1. **Create a Unity Project**  
   - Set up a new **URP** (Universal Render Pipeline) Unity project on **Unity version 6.0.51**.

2. **Install VE2 Package**  
   - Open the **Package Manager**.
   - Click on **Install Package from Git URL**.
   - Paste the following URL:  
     `git+https://github.com/ImperialCollegeLondon/VE2-Distribution.git?path=VE2Installer#main`

3. **Authenticate with Git**  
   - If Git Credential Manager isn't set up on your machine, it should show a popup asking you to log in. Log in with the account used to access the repo (this page!)

4. **Install VE2**  
   - After the package manager has installed the VE2 installer, look in Unity's top menu bar, and navigate to **VE2 > Install VE2**.

5. **Install Samples**
   - Optional: Go to the package manager, find VE2, and install samples - this will give you the VE2 sample scene. You can also use this window to update the VE2 package. 

6. **VE2 Setup Wizard**  
   - Look in unity's top menu bar, navigate to **VE2 > VE2 Quick Setup**
   - Leave all boxes ticked, and select **Setup VE2**

7. **Play the Scene**  
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
   All kinds of errors may pop up here. You may see warnings like:  
   `"Asset Packages/com.ic.ve2installer/package.json has no meta file, but it's in an immutable folder. The asset will be ignored."`

- **Local Server:**
   Expect to see some warnings about the DarkRift server logs not being as expected, differing number of bytes etc

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
- **Instancing Configuration** (max number of players, etc.)  
- **Voice Chat Configuration**  
- **World Build System** (still placeholder)  
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
