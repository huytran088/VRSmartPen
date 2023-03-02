# Conference Paper Reading Notes

## Title
VRySmart: a Framework for Embedding Smart Devices in Virtual Reality

## Year
April 2022

## TL;DR
An framework for intergrating smart devices in virtual reality, help avoiding context switching between VR and external notifications in the real world. This framework was built in Unity, and an user study was conducted, which received positive feedbacks.

## Overall Impression
This is extremely helpful for my current project, since it also includes a GitHub repo for me to test & replicate the application.

## Key Points
- HMDs obscured the real world, making interacting with smart devices while maintaining the immersion is extremely difficult.
- Smart devices mainly used auditory or vibrotacile feedback for notifications of outside events, negatively influence the user's experience
- VRySmart avoided that by creating a virtual representation of smart devices in the VR
- The user study consisted of 4 scenarios: *virtual light saber*, *futuristic slingshot*, *in-VR digital camera*, *messagging application*.
  * 10 participants (24-33 y/o, 8 male, 2 female)
  * The study lasted for about 30~45 minutes
  * 2 parts: guided virtual experience and an interview.
  * After the interview, each of them completed a questionaire about their demographics.
- Mostly positive reviews: *"familiar"*, *"intuitive"*, *"logical"*, and *"useful"*
  * Like being able to taking selfies in VR
  * Some concerns regarding accidentally triggering actions, damaging devices, and privacy.
-Future applications: Gaming, drawing, social media, taking pictures of bystanders, streaming, etc.
-Extend the frameworks to other devices like Google Nest and/or smartwatches.

## Technical Details
- The framework consisted of 2 separate components, which are both built in **Unity 2019.4**: 
  * VR component: coordinating the smart deivce representation into VR
  * Smart device component: The app supported tracking methods and sensor communication.
- There are two tracking methods: *optical marker* and *SLAM*
  * Optical marker: Capture device's rotation and position to coordinate their visual represenation using the camera mounted on the HMD.
  * SLAM: Stands for *simultaneous localization and mapping*. Using the back camera, the smartphone could capture its own real-world position and convert it to shared virtual coordinates.
- For different coordinate spaces, both approach required calibration. For SLAM, it's manual, while it's automatic.
- All events were reported back to the VR component.
- A virtual hand was made using a skin segmentation algorithm to create a separate layer of the hand, helped users interact with the touch screen.
- A VR interface to access the camera stream was provived -> Users could take pictures in the virtual space.

## Notes to Myself
- The SLAM-based tracking method is similar as Inside-out Tracking Controller using phone's camera from Hattori's paper.
- Possiblity of developing writing & drawing application in VR using the framework.
- Intergrating smartwatches into the framework.
- Upgrading to Unity 2022/2023?

---

### Additional Information
- Hattori's paper: [URL](https://dl.acm.org/doi/10.1145/3388770.3407430)

