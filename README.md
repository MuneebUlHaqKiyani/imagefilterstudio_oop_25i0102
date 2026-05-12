# Image Filter Studio - C++ OOP Portfolio Project

This repository contains a console-based C++ Image Filter Studio developed for the CS1004 Object Oriented Programming course at the **National University of Computer & Emerging Sciences**. The application allows users to load real JPG or PNG images, apply a pipeline of custom filters, and save the processed results back to disk.

## ## Project Overview

The "Image Filter Studio" is designed to demonstrate core Object-Oriented Programming (OOP) concepts, including encapsulation, inheritance, polymorphism, and dynamic memory management.

### ### Key Features

* 
**Real Image I/O**: Read and write JPG and PNG files using the `stb_image` and `stb_image_write` libraries.


* 
**Pixel Grid Management**: Images are represented as a 2D grid of `Pixel` objects dynamically allocated on the heap.


* 
**Filter Pipeline**: Apply multiple filters sequentially (e.g., Grayscale followed by Brightness Adjust).


* 
**User Roles**: Distinct functionalities for **Admins** (catalog management, customer oversight) and **Customers** (image processing, history viewing).


* 
**ASCII Preview**: Real-time text-art approximation of the image within the console.



---

## ## Filter Catalog

The project implements 10 unique filters across three categories:

| Category | Filters |
| --- | --- |
| **Pixel Transform** | Grayscale, Invert/Negative, Brightness Adjust, Contrast Stretch, Channel Isolation (R, G, B) 

 |
| **Spatial Filter** | Box Blur ($3 \times 3$) 

 |
| **Geometric** | Flip Horizontal, Flip Vertical 

 |

---

## ## Technical Requirements

* 
**Language**: C++ 


* **Compiler**: g++ (GCC)
* 
**Libraries**: `stb_image.h` and `stb_image_write.h` (included in project folder) 



---

## ## Installation and Running

### ### 1. Clone or Download

Download the project repository as a `.zip` file and extract the contents to your local machine.

### ### 2. Compile

Open your terminal/command prompt in the project directory and run the following command to compile all source files:

```bash
g++ *.cpp -o ImageFilterStudio

```

### ### 3. Run

Execute the compiled program:

**Windows:**

```bash
ImageFilterStudio.exe

```

**Linux/Mac:**

```bash
./ImageFilterStudio

```

---

## ## Usage Guide

1. 
**Login**: Use the Admin credentials (hardcoded) or register as a new Customer.


2. 
**Load Image**: Provide the full system path to a `.jpg` or `.png` file.


3. 
**Build Pipeline**: Select filter IDs to add them to your session.


4. 
**Process**: Apply the pipeline to see the ASCII preview after each step.


5. 
**Save**: Export the final result as a new PNG file, which will be named using your CNIC and a timestamp.



---

## ## OOP Concepts Demonstrated

* 
**Encapsulation**: Private data members in `Pixel` and `Image` classes with controlled access via getters/setters.


* 
**Inheritance**: `Admin` and `Customer` classes extending a base `User` class.


* 
**Polymorphism**: Abstract `Filter` base class with `virtual` methods used to process different filter types at runtime.


* 
**Operator Overloading**: Custom `operator+` for pixel blending and `operator<<` for ASCII rendering.


* 
**Friend Classes**: `FilterSession` is a friend of `Image` to allow direct pixel grid manipulation.
