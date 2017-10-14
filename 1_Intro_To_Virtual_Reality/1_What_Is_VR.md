# What is Virtual Reality?

Virtual Reality is all about creating a synthetic, believable, virtual world. This requires the precise interplay of several hardware and software systems. Not just a headset.

In this section we will overview:

- Displays
- Optics
- Tracking
- Performance
- History

### Optics

The lens of a headset make it possible for your eye to focus on a screen that is extremely close to your face. This makes it hard to see things on the screen because it is blurry. When we look through the lens of a VR headset the image was in nearly perfect focus. By using specialized lens VR headsets focus the light from a near-eye display onto your retina. The lens also greatly magnify the image shown on your phone. You might even be able to see the individual pixels on the display. The size, shape, and placement of these lenses can have a huge impact on the final quality of your VR experience. Each headset manufacturer has to choose a lens that makes the best trade off between field of view, focal length, comfort, optical distortion, and cost.

#### Why do VR headsets have lenses?

VR lenses allow you to focus on a display that is located very close to your eye. Unfortunately, these lenses also greatly magnify the display, reducing its apparent resolution. They also introduce optical distortions in the process.

### Displays

Behind a VR headset's ens, you'll find one or more high resolution OLED displays. Sometimes they are embedded inside the headset like the Vive. Other times, you'll use your phone's display like Google Cardboard or Samsung Gear VR.

It is very important for these displays to have **high resolution**. The magnifying properties of the lenses make the display's pixels much bigger than when they're viewed with the naked eye. We need around 16,000 by 16,000 pixels per eye to have a completely sharp image. For comparison, the Vive currently has 1,080 by 1,200 pixels per eye.

The second important component of a modern VR display is called **low persistence**. Low persistence means that instead of showing you a full image, the display is only showing you a portion of the image in a moment of time. It causes the display to function like a rolling shutter. It only shows your eye a moving slice of the VR world. Why do we only show the slices of an image instead of the full frame? It is because low persistence reduces and in many cases eliminates motion blur. This keeps the image clear when you look around, and it keeps it from smearing together. The individual pixels in a typical OLED display don't change color fast enough to eliminate motion blur. Low persistence fixes that problem by effectively hiding the pixels while they change color. This gives you sharp, consistent, and a believable image when you turn your head. Behind almost every VR headset's lenses you will find high resolution, OLED displays that support low persistence.

#### Why do VR displays use low persistence?

Low persistence causes each pixel in your VR display to illuminate for only a brief period of time. This reduces motion blur when you turn your head. As a side effect, it actually slightly decreases the apparent brightness of the display. And, it has no effect on the display resolution.

### Tracking

VR technology can't exist without tracking. It allows a computer to know where you are in space. To do this, all major VR systems rely on a chip called an **Inertial Measurement Unit** or IMU for short. An IMU enables high speed rotational tracking. This means the chip knows how it is being rotated.

IMU's can't tell where an object is actually located in space, only how it is rotated. In order to tell where objects are located, modern VR systems employ a variety of positional tracking techniques. Sometimes they use cameras, or lasers and precise clocks, or magnetic fields.

VR requires tracking because it's how the system allows your body movements to control the VR world.

### VR Challenges

One of the biggest challenges to VR is simulator sickness. Some VR experiences can give you headaches and make you feel bad. Good VR developers can fix this.

What makes VR uncomfortable? The answer is almost anything that causes a mismatch between your body's internal sense of motion and the data your brain receives from your visual system. If what you see doesn't line up with what you feel, you will be uncomfortable. We will go over ways to prevent simulator sickness when we start developing.
