# PROJECT


This project is a two-axis (Pan-Tilt) camera stabilization and target tracking system capable of following a designated target in real-time. Thanks to a specially designed slip-ring mechanism, the system offers unlimited rotation on the horizontal (Pan) axis, while precisely adjusting the position of the target on the vertical (Tilt) axis. A Raspberry Pi Camera V3 integrated at the tip provides visual feedback to ensure that the target remains centered.


![image url](https://github.com/HalitKosemen/PROJECT/blob/d9289fabf4380c663ba8a7aae9603ce741dd4197/PROJECT/blok_diagram.JPG)




SYSTEM FEATURES:

-Unlimited Pan Motion: One of the most distinctive features of our system is its ability to rotate endlessly on the horizontal axis, thanks to our custom-designed slip-ring mechanism. This mechanism enables continuous transmission of power and control signals without cable tangling issues, allowing uninterrupted target tracking.

![image url](https://github.com/HalitKosemen/PROJECT/blob/edfb45e45943161daf13d053ba86be82c9e8b0fc/PROJECT/slipring.JPG)
![image url](https://github.com/HalitKosemen/PROJECT/blob/edfb45e45943161daf13d053ba86be82c9e8b0fc/PROJECT/slip_ring2.jpg)
![image url](https://github.com/HalitKosemen/PROJECT/blob/edfb45e45943161daf13d053ba86be82c9e8b0fc/PROJECT/ring.JPG)

-Precise Two-Axis Control: The Pan and Tilt axes are controlled by stepper motors, allowing the target's position to be adjusted with millimeter-level precision in both horizontal and vertical planes.

![image url](https://github.com/HalitKosemen/PROJECT/blob/edfb45e45943161daf13d053ba86be82c9e8b0fc/PROJECT/top.JPG)

-Visual Target Tracking: The Raspberry Pi Camera V3 mounted at the end of the system provides a high-resolution video stream. Our OpenCV-based software running on a PC analyzes this stream to extract the real-time position of the target.


-PID Control: Precise motor movements on the Pan and Tilt axes are managed using an optimized PID (Proportional-Integral-Derivative) control algorithm. This ensures fast, stable, and accurate locking onto the target. The PID coefficients can be easily adjusted during system operation.


Custom Driver Board and Power Management: The system uses a custom-designed driver board (PCB) to precisely control the stepper motors and reliably power the entire system. This board receives STEP and DIRECTION control signals from the Raspberry Pi and transmits them to the motors to manage their stepping movements.
Most importantly, since the power supply for all components — including the Raspberry Pi — passes through this board, the power traces and widths on the PCB have been carefully designed to support current loads of up to 5 Amps.
This ensures stable and safe operation even under high power demands, while preventing potential issues such as overheating and voltage drops.

![image url](https://github.com/HalitKosemen/PROJECT/blob/3179402857f6a7a159d1b50bbcf4538313963cb2/PROJECT/pcb.JPG)
![image url](https://github.com/HalitKosemen/PROJECT/blob/3179402857f6a7a159d1b50bbcf4538313963cb2/PROJECT/5amper.JPG)
