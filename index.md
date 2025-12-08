---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
---
For my project, I created a slideshow that shows the Irish, Nigerian, and English national flags on a VGA monitor using Verilog. The design runs on a Basys3 FPGA and draws each flag before switching to the next.
## **Template VGA Design**
### **Project Set-Up**
![VGASync Source Screenshot](VGAsource.png)
### **Template Code**
The project started with Verilog templates that handled the basic pipeline. VGASync.v generates the 640×480 VGA timing signals (hsync, vsync, vid_on ) and provides pixel coordinates (row, col). that determined when each frame began. VGATop.v connected the timing logic to a colour cycle module, which was used to test if the output worked. I altered the colour cycle module with code to display the Nigeria, Ireland, and England flags in a timed slideshow
