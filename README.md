# Text Segmentation Tool - C++ NLP Project

A **custom text segmentation tool** that automatically divides large text into meaningful segments using dynamic programming and word similarity metrics. This project demonstrates **NLP algorithm design, parameter optimization, and GUI integration** in C++.

---

## Features

- **Dynamic Text Segmentation:** Implements a dynamic programming-based segmentation algorithm that considers:
  - Segment length (`μ`)  
  - Segment deviation (`σ`)  
  - Weight (`γ`) between length and density  
  - Density exponent (`r`) for similarity normalization  

- **Text Preprocessing:**  
  - Sentence splitting and cleaning  
  - Tokenization and lowercasing  
  - Punctuation removal  

- **Interactive GUI:** Built with **FLTK**, featuring:  
  - Real-time text input  
  - Adjustable segmentation parameters (`μ`, `σ`, `γ`, `r`)  
  - Segmented output with colored highlights for readability  
  - Segment headers for clarity  

- **Algorithm Optimization:**  
  - Efficient similarity computation between sentences  
  - Handles multi-sentence documents with dynamic programming for minimal segmentation cost  

---

## Demo Screenshot

![Demo Screenshot](demo_screenshot.png)  <!-- Replace with actual screenshot -->

---

## Getting Started

### Prerequisites

- C++17 or higher
- [FLTK](https://www.fltk.org/) library installed
- Standard C++ compiler (e.g., g++, clang, Visual Studio)

### Build Instructions

1. Clone the repository:

```bash
git clone https://github.com/your-username/text-segmentation-cpp.git
cd text-segmentation-cpp
Compile the project (example with g++):

bash
Copy code
g++ main.cpp -o TextSegmenter -lfltk -lfltk_images -lX11
Run the application:

bash
Copy code
./TextSegmenter
Usage
Enter your text in the Input Text field.

Adjust the parameters:

μ (average segment length)

σ (length deviation)

γ (weight between length and density)

r (density exponent)

Click Segment Text to visualize segmented output.

Use Clear to reset the output field.

Project Highlights
Fully custom NLP algorithm implemented in C++ without relying on pre-built ML libraries.

Demonstrates algorithmic thinking, text processing, and GUI programming.

Ideal for showcasing AI/ML problem-solving and software development skills in a resume or portfolio.

Potential Improvements
Add automatic evaluation against a labeled dataset.

Implement additional similarity measures (e.g., cosine similarity with embeddings).

Expand GUI to allow saving segmented text.
