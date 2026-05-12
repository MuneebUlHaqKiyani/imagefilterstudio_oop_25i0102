# Image Filter Studio - C++ OOP Portfolio Project

This console-based C++ Image Filter Studio was developed for the CS1004 Object Oriented Programming course at the National University of Computer & Emerging Sciences. It allows users to load real JPG or PNG images, process them through a pipeline of filters, and save the results back to disk.

## Project Overview

The application serves as an OOP portfolio, demonstrating every concept from raw pointers and dynamic memory to polymorphism and virtual functions.

### Core Features

* 
**Real Image I/O**: Loads and decodes JPG/PNG pixels into a grid and writes them back using the `stb_image` library.


* 
**Dynamic Pixel Grid**: Images are stored as a 2D array of `Pixel` objects on the heap using `Pixel`.


* 
**Filter Pipeline**: Chains multiple filters together, where each filter runs on the output of the previous one.


* 
**ASCII Preview**: Generates a text-art approximation of the image in the console using brightness-to-character mapping.


* 
**User Management**: Includes an Admin role for catalog management and a Customer role for image processing.



---

## Filter Catalog

The studio includes 10 mandatory filters categorized as follows:

| Category | Filter Name | Description |
| --- | --- | --- |
| **Pixel Transform** | Grayscale, Invert, Brightness Adjust, Contrast Stretch, RGB Channel Filters | Manipulates individual pixel values.

 |
| **Spatial Filter** | Box Blur ($3 \times 3$) | Averages a pixel with its 8 neighbors while handling edges.

 |
| **Geometric** | Flip Horizontal, Flip Vertical | Mirrors the image by swapping pixel rows or columns.

 |

---

## Technical Specifications

* 
**Language**: C++ 


* **Compiler**: g++
* 
**OOP Concepts**: Abstract base classes, pure virtual methods, friend classes, operator overloading (`+`, `<<`), and deep copy constructors.


* 
**Data Persistence**: Uses `.txt` files to store customer data, filter catalogs, and session history.



---

## Installation and Execution

### 1. Download and Extract

Download the project zip file and extract it into a folder. Ensure `stb_image.h` and `stb_image_write.h` are in the project directory.

### 2. Compile

Open your terminal in the project directory and run:

```bash
g++ *.cpp -o ImageFilterStudio

```

### 3. Run

Execute the program:

* **Windows**: `ImageFilterStudio.exe`
* **Linux/Mac**: `./ImageFilterStudio`

---

## Submission Requirements

* 
**Deadline**: 03rd-May-2026, 5:00 PM.


* 
**Format**: Submit a .zip file named `i21-XXXX_Name_Section.zip`.


* 
**Policy**: Strict plagiarism rules apply; non-running code receives zero marks.
