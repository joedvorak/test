
Welcome to the test wiki! This is a test to see what form would work best for our documentation. The goal here is to capture all the information to create a good engineering design file.

# Test Project
Created by Joe Dvorak, BAE 305 Team, Others

# Summary
This project doesn't do anything. I'm just seeing how the formatting works. It seems okay, but we will see. It allows code input and links to videos. After some experiments, it should work perfect for the class. How does it compare to GitHub Pages?

# Equipment and Materials Used
* Arduino Uno
* CAN SPI Click
* Kubota Engine

# Work Performed
Here we describe the work we did to get our outcome.
Images?

# Outcome and Design Discussion
How did it work? Did we achieve our goals? Do you have hints for others?

Here is a chuck of code:

```Arduino
      eng_RPM++;
      nSrcAddr = j1939.GetSourceAddress();
      msgShort[3]=eng_RPM&0xFF;
      msgShort[4]=(eng_RPM>>8)&0xFF;
      j1939.Transmit(6, 59999, nSrcAddr, 0x43, msgShort, 5);
      j1939.Transmit(6, 0xFEEE, nSrcAddr, 0x11, msgShort, 8);
      j1939.Transmit(6, 0xF004, nSrcAddr, 0x11, msgShort, 8);
      //j1939.Transmit(6, 0xEA43, nSrcAddr, 0x43, msgShort, 8);
      nCounter = 0;
```

# Final Design
Point to the code embedded within this project! Yea! No more PDFs of code! Final Schematics and Design files listed here!
