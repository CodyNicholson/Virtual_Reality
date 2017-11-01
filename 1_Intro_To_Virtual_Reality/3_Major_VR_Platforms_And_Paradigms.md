# Major Virtual Reality Platforms & Paradigms

### 3-DOF Vs 6-DOF

One of the big differences between mobile and desktop VR platforms is the concept of 3-DOF versus 6-DOF tracking. DOF is short for Degrees of Freedom. It deals with how accurately the VR system can track you. For a VR headset it is the difference between knowing only where you're looking and where you're looking and located in the room. Three degrees of freedom means your head can be tracked when it rotates along the x-axis, the y-axis, and the z-axis. This is what most mobile VR platforms do. Six degrees of freedom means that in addition to tracking your head on all three axises, you will also be tracked as you move around the room. **High NVR** systems allow you to do this.

*In other words, your head rotation and position is tracked in 6-DOF, while only your head rotation is tracked in 3-DOF.*

### How IMUs Enable 3-DOF Tracking

VR headsets can quickly and accurately detect rotation. The do this using a **Inertial Measurement Unit**, or IMU for short. An IMU is a tiny sensor that is really good at quickly and accurately detecting rotations. It does this by combining the data from an onboard accelerometer, magnetometer, and gyroscope. Basically it is using gravity and the Earth's magnetic field to constantly infer which way it is pointed. By using some fancy math, and IMU is able to detect the direction it is facing. That is how 3-DOF works. Sometimes an IMU is embedded inside your VR headset, and sometimes it is inside your phone instead. No matter what, all modern 3-DOF tracking uses some kind of IMU.

### Intro to 6-DOF Tracking

For 6-DOF tracking there isn't some standard sensor that we can use to quickly figure out where things are located. Almost every high-end VR headset uses a different kind of optical tracking system. However, there are all different kinds of other approaches that can also be used. There are tracking systems using magnetism and acoustics that are also viable. Even among optical tracking systems there is a lot of variation.

There are many different ways to do 6-DOF positional tracking. We will look at how two of the major VR headsets do it, starting with the Oculus Rift.

The Oculus uses a tracking system called **Constellation**. Behind the exterior fabric, the Rift has a large number of infrared LEDs. Each LED is blinking really fast in a specific pattern. There is also a separate camera that is placed somewhere nearby. The camera captures the light patterns, and a computer program builds up a model of the light positions. That program then tried to fit a 3D model of the Rift onto the 2D model it sees from the camera. Based on this 3D model - the measurements from an internal IMU - it calculates your head position. It tries to do this extremely quickly and accurately. None of the tracking systems are perfect. Constellation is pretty good and fairly cheap.

The HTC Vive uses a different tracking system called **Lighthouse**. It also uses infrared light, but it uses infrared lasers. It works by measuring the time it takes for a laser to sweep horizontally and vertically across a fast photosensor. It is actually a similar principle to how a ships navigate by using time measurements between lighthouse flashes. If you look closely, both the Vive headset and controllers are covered with little circular indentations for the photosensors. A Vive base station is constantly sweeping the room with a laser that hits the photosensors. The sweep times are used to determine their positions in space. It uses this data and combines it with readings from an embedded IMU to determine where your head and hands are located.

#### Remember that an IMU is most commonly used for rotational tracking. What physical property is most commonly used for positional tracking?

Even though all of these physical properties can be used for positional tracking in a 6-DOF system, modern VR devices mostly use optics. Cameras and photo sensors are the popular choices for modern VR positional tracking

### Key Differences Between Mobile & Desktop Virtual Reality

#### Mobile VR

- IMU Tracking, only three degrees of freedom. Mobile VR devices are phone based. It can only track your head's rotation, not position.
- Untethered - meaning it has no wire connecting the headset to a computer
- Less powerful than desktop in terms of graphic performance

#### Desktop VR

- Full 6-DOF tracking, Optical & IMU Tracking
- Tethered - a long cable runs from the headset to the PC
- More powerful, lots of computing power, higher visual quality
- Can use hand controllers

### VR Development Platforms

There are two primary ways of rendering 3D environments. You can write code, or you can use a graphical editor-based environment. You could also do both. We will start by using a game engine called **Unity**. A game engine is a software framework that makes it easier to develop games. The goal is to reduce iteration time and overhead as much as possible. Short iteration times are crucial because VR requires quick experimentation. We don't know everything about this medium. Game engines often provide: 3D rendering, Physics, Sound, Scripting, Animation, Asset Management, and more. It is a package of tools that results in shorter development times. Some of the other big game engines are Unreal Engine, CryEngine, Lumberyard, and more.

To contrast game engines, you can also build game engines using native tools likes C++, OpenGL, and DirectX. These tools allow you to build your VR software using the raw materials of the computer graphics world. Instead of using prepackaged tools and a game engine, native development requires you to integrate every component you want to use. The result is a much more flexibility and increased performance, but much longer development times. When you need performance, this is the best option. Or you might use native development when you want to build a framework for others to use.

The last VR development option out there that we will talk about is Web Browsers. It currently isn't good enough for production use, but it is constantly improving. For now we have to choose between a game engine and native development.
