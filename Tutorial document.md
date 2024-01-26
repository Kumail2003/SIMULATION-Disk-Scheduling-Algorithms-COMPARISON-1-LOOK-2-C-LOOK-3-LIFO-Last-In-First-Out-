# Disk Scheduling Algorithms Simulation

Welcome to the tutorial on Disk Scheduling Algorithms Simulation. This guide will walk you through the features, customization options, and algorithms implemented in the simulation project.

## 📚 **Table of Contents**
1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
   - [Installation](#installation)
   - [Dependencies](#dependencies)
3. [Usage](#usage)
   - [Randomly Generate Input](#randomly-generate-input)
   - [Perform Simulation](#perform-simulation)
   - [Toggle Simulation](#toggle-simulation)
4. [Customization](#customization)
   - [Styles](#styles)
   - [Extending Algorithms](#extending-algorithms)
5. [Simulation Results](#simulation-results)
   - [Graph](#graph)
   - [Table](#table)
6. [Explanation of Algorithms](#explanation-of-algorithms)
   - [LOOK Algorithm](#look-algorithm)
   - [C-LOOK Algorithm](#c-look-algorithm)
   - [LIFO Algorithm](#lifo-algorithm)
7. [Step-by-Step Walkthrough](#step-by-step-walkthrough)
8. [Additional Information](#additional-information)
   - [Troubleshooting](#troubleshooting)
   - [Contributing](#contributing)
9. [Group Members](#group-members)

## 🌟 **Introduction**
The Disk Scheduling Algorithms Simulation project offers a visual representation of disk scheduling algorithms, enabling you to compare and analyze the performance of LOOK, C-LOOK, and LIFO algorithms.

## 🚀 **Getting Started**
### [Installation]
- Clone or download the project from the repository.
- Open the `os.html` file in a modern web browser.

### [Dependencies]
The simulation utilizes the Plotly library for graph visualization, included via a CDN link in the HTML file.

## 💡 **Usage**
1. **Random Input Generation:**
   - Click the "Randomly Generate Input" button to quickly set initial positions and request orders for testing.

2. **Simulation Execution:**
   - Click "Perform Simulation" to initiate the disk scheduling simulation based on your chosen algorithm.

3. **Simulation Toggle:**
   - Click "Toggle Simulation" to pause or resume the simulation at any point.

## 🎨 **Customization**
To customize the appearance of the simulation, you can modify the CSS in the `<style>` section of the HTML file. This allows you to adjust colors, fonts, or layout according to your preferences.

### [Extending Algorithms]
The simulation is designed to be easily extended. By modifying the `diskSchedulingAlgorithm` function in the JavaScript code, you can adapt or extend the behavior of the disk scheduling algorithms to suit your needs.

## 📊 **Simulation Results**
The simulation provides two ways to view the results: a graph and a table.

### [Graph]
The graph represents the seek time on the x-axis and the number of cylinders accessed on the y-axis. Each point on the graph corresponds to a simulation step, and text annotations provide additional details.

### [Table]
The table displays the seek times and cylinders accessed at each step of the simulation, including the average seek time.

## 📘 **Explanation of Algorithms**
The simulation includes three different disk scheduling algorithms: LOOK, C-LOOK, and LIFO.

1. **LOOK Algorithm:**
   - The LOOK algorithm sorts the requests and moves the disk head towards higher or lower cylinder numbers, changing direction when necessary.

2. **C-LOOK Algorithm:**
   - The C-LOOK algorithm is similar to LOOK, but it uses circular movement to prevent unnecessary head movement when reaching disk boundaries.

3. **LIFO Algorithm:**
   - The LIFO algorithm processes requests in reverse order, starting from the last request.

## 🚶 **Step-by-Step Walkthrough**
To use the simulation, follow these steps:

1. Open `os.html` in a web browser.
2. Click "Randomly Generate Input" to quickly generate test data.
3. Click "Perform Simulation" to observe the algorithm in action.
4. Analyze the graph and table to view the results.

## ℹ️ **Additional Information**
### [Troubleshooting]
If you encounter any issues or have questions, please refer to the troubleshooting section in the README file.

### [Contributing]
If you'd like to contribute to the project, follow the guidelines outlined in the CONTRIBUTING.md file.

## **Group Members**
Introducing the skilled individuals who have made valuable contributions to this project:

1. - **Name:** Muhammad Kumail
   

2. - **Name:** Muhammad Rehan Maqbool

3. - **Name:** Ahmad Hassan
   
