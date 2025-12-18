# Water-Tank-Trapping-Rain-Water-Visualization
Water Tank (Trapping Rain Water) Visualization
📌 Overview

This project demonstrates the Water Tank (Trapping Rain Water) problem using a frontend-only web application built with HTML, CSS, and Vanilla JavaScript.

The application:

Accepts block heights as input

Calculates the total units of water trapped between blocks

Visually represents blocks and trapped water using SVG graphics

This project is designed as an interview assignment to showcase algorithmic thinking + frontend visualization skills.

🧩 Problem Statement

Given an array of non-negative integers representing block heights, calculate how much water can be trapped between the blocks after rainfall.

Rules:

Each element represents the height of a block

Water can be trapped only if there are taller blocks on both sides

The total trapped water is the sum of water stored at each index

▶ Example
Input
[0, 4, 0, 0, 0, 6, 0, 6, 4, 0]

Output
Total Trapped Water = 18 units

🎯 Objective

Calculate the total trapped rainwater

Visualize blocks and trapped water clearly

Build a pure frontend solution without external libraries

🏗 Application Features

✅ User input for block heights (comma-separated)

✅ Efficient water calculation using Two-Pointer technique

✅ SVG-based visualization for blocks and water

✅ Real-time calculation and rendering

✅ Clean and responsive UI

💡 Solution Approach (Easy Explanation)
Algorithm Used: Two-Pointer Technique

We use two pointers:

left starting from the beginning

right starting from the end

We also track:

leftMax → highest block seen from the left

rightMax → highest block seen from the right

Key Logic:

If the left block is smaller, water depends on leftMax

If the right block is smaller, water depends on rightMax

Water at each index = min(leftMax, rightMax) - height[i]

This method is efficient and avoids extra loops.

🧠 Algorithm Steps

Initialize two pointers (left, right)

Track maximum heights on both sides

Move the pointer with smaller height

Calculate trapped water at each position

Store water values for visualization

Display total trapped water

📊 Visualization Explanation

🟫 Grey blocks represent the heights entered by the user

💧 Blue blocks represent trapped water

SVG ensures smooth and scalable visualization

🖥 Technologies Used

HTML5

CSS3

Vanilla JavaScript

SVG for visualization

⏱ Complexity Analysis

Time Complexity: O(n)

Space Complexity: O(n) (for water storage and visualization)

🌍 Real-World Applications

This problem has practical use in:

🏗 Civil Engineering – water accumulation analysis

🌧 Rainwater Harvesting Systems

🏙 Urban Drainage Planning

🧮 Algorithm & Data Structure Learning

🎓 Technical Interviews

🧪 How to Run the Project

Clone the repository

Open water.html in any modern browser

Enter block heights (comma-separated)

Click Calculate & Visualize

View trapped water and visualization instantly
