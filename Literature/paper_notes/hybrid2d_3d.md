# [A Hybrid 2D-3D Tangible Interface for Virtual Reality](https://doi.org/10.1145/3450618.3469166)

_August 2021_

tl;dr: A novel input method for a hybird 2D-3D tangible VR interface, combining a smartphone and a VR controller.

#### Overall Impression
Interesting idea. I intend to use a smartphone as a controller for writting in virtual 3D space. This article is a good start.
#### Key Points
* Many controllers use outside-in tracking for HMDs
* An inside-out tracking, which can detect 6DoF, is studied.
* A raycasting system in VR/AR using image recognition on a smartphone


#### Technical details
* The 6DoF synchronization method, using “_Cloud Anchor_” in ARCore:
* Two smartphones are used: one is attached to the HMD, another is the controller
* The synchronization is performed 30 times/sec.
* A “_Fix button_” is provided to fix the CG objects displayed in the space, and adjust the 6DoF of the controller to the desired position.

#### Notes
- The controller, as seen from the display, was out of position with the actual position.
- Could be solved by pressing the fix button.
- Can the position fixed automatically without pressing a button?


