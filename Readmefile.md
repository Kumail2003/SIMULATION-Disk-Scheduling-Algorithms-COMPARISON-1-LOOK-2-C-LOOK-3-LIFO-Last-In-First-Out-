# Disk Scheduling Algorithms Simulation

This HTML file (`os.html`) presents a comprehensive tool for simulating and comparing different disk scheduling algorithms. The simulation includes LOOK, C-LOOK, and LIFO (Last-In First-Out) algorithms, allowing users to explore their performance characteristics under various scenarios.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [Usage](#usage)
5. [Customization](#customization)
6. [Simulation Results](#simulation-results)
7. [Group Members](#group-members)

## Introduction

Efficient disk access is crucial for optimal system performance in the realm of operating systems. Disk scheduling algorithms play a vital role in determining the order in which disk requests are fulfilled. This simulation aims to illustrate, compare, and analyze the behaviors of LOOK, C-LOOK, and LIFO algorithms based on the initial position of the disk head and the sequence of disk requests.

## Features

1. **Visualization of Algorithm Performance:**
   The core of this simulation lies in its graphical representation of disk scheduling algorithm performance. Seek time is plotted on the x-axis, while the number of cylinders accessed is plotted on the y-axis. Each point on the graph corresponds to a step in the algorithm execution, providing a visual journey through the disk access process.

2. **Random Input Generation:**
   To facilitate quick and diverse testing, the "Randomly Generate Input" button allows users to set random initial positions and request orders. This feature assists in exploring algorithm performance under different starting conditions.

3. **Dynamic Updates:**
   The graph dynamically updates during the simulation, offering a step-by-step visualization of the algorithm's execution. Users can observe how the disk head moves and accesses cylinders at each iteration.

4. **Tabular Display:**
   Simulation results are presented in a tabular format, providing a detailed breakdown of seek times and the corresponding cylinders accessed at each step. This tabular display offers a structured view of the algorithm's progression.

5. **Calculation of Average Seek Time:**
   After the simulation is completed, the tool will calculate and display the average seek time. This metric provides a quantitative measure of the overall efficiency of the disk scheduling algorithm.

## Getting Started

To begin the simulation journey:
1. Open the HTML file in a web browser.

## Usage

1. **Randomly Generate Input:**
   Click the "Randomly Generate Input" button to set random initial positions and request orders. This feature enables quick and diverse testing scenarios.

2. **Perform Simulation:**
   Click the "Perform Simulation" button to start the disk scheduling simulation. Choose the desired algorithm from the available options, and the simulation will dynamically illustrate the behavior of the algorithm.

3. **Toggle Simulation:**
   The "Toggle Simulation" button allows users to pause or resume the simulation. This feature is particularly useful for closely examining specific steps or temporarily halting the simulation.

## Customization

The code is designed to be flexible and easily customizable to meet specific requirements. Users can adjust the simulation speed, modify styles, or extend the algorithms according to their needs.

1. **Customizing Styles:**
   Feel free to customize the visual styles of the simulation by modifying the CSS within the `<style>` section of the HTML file.

2. **Extending Algorithms:**
   For users interested in exploring different disk scheduling algorithms or modifying existing ones, the `diskSchedulingAlgorithm` function in the JavaScript code can be extended. This enables the implementation of custom logic or the integration of additional algorithms.

## Simulation Results

The simulation outcomes are showcased in two complementary formats:

1. **Graph:**
   The visual depiction offers a user-friendly visualization of the seek time and the number of cylinders accessed. Each data point on the graph corresponds to a specific step in the simulation, and textual annotations provide in-depth insights into each step.

2. **Table:**
   A systematic breakdown presents seek times and cylinders accessed at each step in a tabular format. Furthermore, the tool computes and presents the average seek time, offering a quantitative summary of the algorithm's effectiveness. This combination of graphical and tabular representations ensures a comprehensive grasp of the simulation results.

## Group Members

Introducing the skilled individuals who have made valuable contributions to this project:

1. **Muhammad Kumail**

2. **Muhammad Rehan Maqbool**
   

3. **Ahmad Hassan**
   
