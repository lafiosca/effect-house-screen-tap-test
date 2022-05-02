# Screen Tap Test

This is a project demonstrating touch gesture math in Effect House. It calculates a world position to move a sphere where the user taps.

## iPhone bug

I think I have discovered a serious platform-specific bug in the gesture handling (Screen Tap) or screen position math (World to Screen). Specifically, it appears that the touch math in this project does not work correctly on certain newer iPhone devices, offsetting the position a bit vertically. See this video for a demonstration: https://www.youtube.com/watch?v=lhSnm8huEug

With the help of @lauragouillon, @ひろゆき, and @Mingus, we have tested the effect on several devices.

On these devices, we experienced the buggy behavior:

- iPhone 13 Pro running iOS 15.4.1 [(video)](https://www.youtube.com/watch?v=lhSnm8huEug)
- iPhone 13 Pro running iOS 15.2
- iPhone 12 Pro Max [(photo)](media/iPhone%2012%20Pro%20Max.jpg) [(screenshot)](media/iPhone%2012%20Pro%20Max%20screenshot.jpg)
- iPhone 11 running iOS 15.4.1 [(video)](media/iPhone 11.mov)

On these devices, we saw the intended behavior:

- iPhone 11 running iOS 15.1
- iPhone 8 running iOS 14.7.1 [(video)](https://www.youtube.com/watch?v=lhSnm8huEug)
- Nokia 3.4 running Android 11 [(video)](https://www.youtube.com/watch?v=lhSnm8huEug)

The effect also behaves as intended in the Effect House preview.

The same bad behavior occurs with Finger Touch 1-Point as well.
