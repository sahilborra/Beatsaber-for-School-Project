Transcribed using Gemini

### Fundamentals of Vision Hardware



**Resolution & FPS**

* Resolution dictates spatial detail (pixel grid count).


* FPS dictates how many snapshots are taken per second.



**Why do videos blur?**

* Motion blur happens when an object moves across the camera's sensor while the shutter is open.


* If the shutter speed is too slow relative to the speed of the saber, the object moves across multiple pixels within a single exposure, making a "streak".



**Rolling vs Global Shutter**

* **Rolling Shutter:** Reads the light sensors on the camera line-by-line (top to bottom). Causes geometric distortion (skewing) on fast moving objects, because the bottom of the frame is captured slightly later than the top.


* **Global Shutter:** Exposes every single pixel at the same time. Captures fast movements perfectly without warping.



**Why Global Shutter Cameras are Rarer & Lower Resolution**

* **Circuitry Complexity:** Each pixel requires its own memory capacitor to hold data.


* **High Amounts of Data:** With higher resolutions, there would be too much data being outputted per second, which is why they tend to be low resolution (0.3-2 Mega Pixels).



---

### Design Decisions & Justifications



**Decision 1: Rolling vs Global Shutter**

* **Decision:** Global shutter.


* **Justification:** A saber moved by a player undergoes rapid acceleration. A rolling shutter would bend or distort the shape of the saber in the video, causing issues when estimating its position.



**Decision 2: Minimum Resolution & Frame Rate**

* **Decision:** 480p at 60 FPS.


* **Justification:** Using high resolutions lead to extremely large volumes of data being transferred, leading to strains in processing.
