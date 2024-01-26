<!DOCTYPE html>
<html>

<head>
    <title>SIMULATION: Disk Scheduling Algorithms COMPARISON 1) LOOK 2) C-LOOK 3) LIFO (Last-In First-Out)</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f0f0; /* Light gray background */
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh; /* Set minimum height to fill the viewport */
        }

        #myPlot {
            width: 100%;
            max-width: 800px;
            margin-top: 20px;
        }

        #controls {
            margin-top: 20px;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            background-color: #ffffff; /* White background for controls */
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Soft box shadow */
        }

        label {
            margin: 5px;
            font-size: 16px;
            color: #333333;
        }

        input {
            padding: 10px;
            margin: 5px;
            border: 1px solid #1976D2;
            border-radius: 6px;
            font-size: 14px;
            transition: border-color 0.3s ease; /* Add transition for input border */
        }

        input:focus {
            border-color: #2196F3; /* Change border color on focus */
        }

        button {
            background-color: #2196F3; /* Material blue color */
            color: white;
            padding: 12px 24px;
            margin: 5px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            transition: background-color 0.3s ease, color 0.3s ease; /* Add transitions for button */
            font-size: 16px;
        }

        button:hover {
            background-color: #1565c0;
            color: #ffffff;
        }

        select {
            padding: 10px;
            margin: 5px;
            color: #333333;
            background-color: white;
            border: 1px solid #1976D2;
            border-radius: 6px;
            font-size: 14px;
            transition: border-color 0.3s ease; /* Add transition for select border */
        }

        select:focus {
            border-color: #2196F3;
        }

        #dataTableContainer {
            overflow-x: auto;
            max-width: 800px;
            margin-top: 20px;
        }

        #dataTable {
            width: 100%;
            border-collapse: collapse;
        }

        th, td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
            font-size: 14px;
        }

        th {
            background-color: #f2f2f2;
        }
    </style>
</head>

<body>

    <div id="myPlot"></div>

    <div id="controls">
        <label for="initialPosition">Initial Position:</label>
        <input type="number" id="initialPosition" required>

        <label for="requestOrder">Request Order (comma-separated):</label>
        <input type="text" id="requestOrder" required>

        <button onclick="generateRandomInput()">Randomly Generate Input</button>

        <label for="algorithm">Select Algorithm:</label>
        <select id="algorithm">
            <option value="look">LOOK</option>
            <option value="cLook">C-LOOK</option>
            <option value="lifo">LIFO</option>
        </select>

        <button onclick="performSimulation()">Perform Simulation</button>
        <button onclick="toggleSimulation()">Toggle Simulation</button>
    </div>

    <div id="dataTable"></div>

    <script>
        let seekTimeArray = [];
        let cylindersAccessedArray = [];
        let initialPositionMarker = [];
        let simulationSpeed = 1000; // Delay between steps in milliseconds
        let simulationPaused = false;
        let totalInitialMovement = {
            look: 0,
            cLook: 0,
            lifo: 0
        };

        let animationFrame;
        function updateGraph() {
            const data = [{
                x: seekTimeArray,
                y: cylindersAccessedArray,
                mode: "markers+lines+text", // Include text in the mode
                type: "scatter",
                name: "Algorithm Performance"
            }];
        
            // Add a marker for the initial position if available
            if (initialPositionMarker.length > 0) {
                data.push({
                    x: [initialPositionMarker[0]],
                    y: [initialPositionMarker[1]],
                    mode: "markers",
                    type: "scatter",
                    marker: {
                        color: 'red', // Initial position marker color
                        size: 10
                    },
                    name: "Initial Position"
                });
            }
        
            // Add text annotations for request order numbers
            for (let i = 0; i < cylindersAccessedArray.length; i++) {
                data.push({
                    x: [seekTimeArray[i]],
                    y: [cylindersAccessedArray[i]],
                    text: [cylindersAccessedArray[i]], // Display cylinder accessed number
                    mode: "text",
                    type: "scatter",
                    textposition: 'bottom center', // Adjust text position
                    textfont: {
                        family: 'Arial',
                        size: 12,
                        color: 'black'
                    }
                });
            }
        
            const layout = {
                xaxis: {
                    title: "Seek Time (ms)"
                },
                yaxis: {
                    title: "Number of Cylinders Accessed"
                },
                title: "Disk Scheduling Performance Visualization"
            };
        
            Plotly.newPlot("myPlot", data, layout);
        }
        

        function generateRandomInput() {
            const initialPositionInput = document.getElementById('initialPosition');
            const requestOrderInput = document.getElementById('requestOrder');

            initialPositionInput.value = Math.floor(Math.random() * 200);
            requestOrderInput.value = Array.from({
                length: 5
            }, () => Math.floor(Math.random() * 200)).join(',');

            
        }

        async function performSimulation() {
            let initialPosition = parseInt(document.getElementById('initialPosition').value);
            let requestOrder = document.getElementById('requestOrder').value.split(',').map(Number);
            let algorithm = document.getElementById('algorithm').value;

            // Clear previous data
            seekTimeArray = [];
            cylindersAccessedArray = [];
            initialPositionMarker = [];

            // Reset total initial movement
            totalInitialMovement = {
                look: 0,
                cLook: 0,
                lifo: 0
            };

            // Placeholder: Implement disk scheduling algorithm logic here
            // Modify seekTimeArray, cylindersAccessedArray, and totalInitialMovement based on the algorithm and input
            await diskSchedulingAlgorithm(algorithm, initialPosition, requestOrder);

            // Update graph
            updateGraph();

            // Log total initial movement for each algorithm
            console.log('Total Initial Movement - LOOK:', totalInitialMovement.look);
            console.log('Total Initial Movement - C-LOOK:', totalInitialMovement.cLook);
            console.log('Total Initial Movement - LIFO:', totalInitialMovement.lifo);

                        // Display the table with seek times
                        updateTable();
                    }
            
                    async function diskSchedulingAlgorithm(algorithm, initialPosition, requestOrder) {
                        // Add initial position to arrays
                        seekTimeArray.push(0);
                        cylindersAccessedArray.push(initialPosition);
            
                        // Add initial position marker if the algorithm is 'look' or 'cLook'
                        if (algorithm === 'look' || algorithm === 'cLook') {
                            initialPositionMarker = [0, initialPosition];
                        }
            
                        if (algorithm === 'look') {
                            requestOrder.sort((a, b) => a - b); // Sort requests
                            let currentPosition = initialPosition;
                            let direction = 1; // 1 for moving towards higher cylinder numbers, -1 for moving towards lower cylinder numbers
            
                            for (const request of requestOrder) {
                                const seekTime = Math.abs(request - currentPosition);
                                seekTimeArray.push(seekTime);
                                cylindersAccessedArray.push(request);
                                currentPosition = request;
            
                                // Check if there are requests in the current direction
                                const requestsInDirection = requestOrder.filter(r => (direction === 1 ? r > currentPosition : r < currentPosition));
            
                                if (requestsInDirection.length === 0) {
                                    // Change direction only if there are no more requests in the current direction
                                    const remainingRequests = requestOrder.filter(r => r > currentPosition);
                                    if (remainingRequests.length > 0) {
                                        direction = 1;
                                        requestOrder.sort((a, b) => a - b); // Sort requests in ascending order
                                    } else {
                                        direction = -1;
                                        requestOrder.sort((a, b) => b - a); // Sort requests in descending order
                                    }
                                }
            
                                // Remove the processed request from the array
                                requestOrder = requestOrder.filter(r => r !== request);
            
                                // Accumulate total initial movement
                                totalInitialMovement.look += seekTime;
            
                                await animateSimulationStep(); // Introduce animation delay
                            }
                        } else if (algorithm === 'cLook') {
                            requestOrder.sort((a, b) => a - b); // Sort requests
                            const index = requestOrder.findIndex(request => request > initialPosition);
                            const sortedRequests = [...requestOrder.slice(index), ...requestOrder.slice(0, index)];
                        
                            let currentPosition = initialPosition;
                        
                            for (let i = 0; i < sortedRequests.length; i++) {
                                const request = sortedRequests[i];
                                if (simulationPaused) return;
                        
                                const seekTime = Math.abs(request - currentPosition);
                                seekTimeArray.push(seekTime);
                                cylindersAccessedArray.push(request);
                                currentPosition = request;
                        
                                // Accumulate total initial movement
                                totalInitialMovement.cLook += seekTime;
                        
                                // Remove the processed request from the array
                                sortedRequests.splice(i, 1);
                                i--;
                        
                                // Check if it's the last request and there are more requests
                                if (i === sortedRequests.length - 1 && sortedRequests.length > 0) {
                                    i = -1; // Reset i to process the next request
                                }
                        
                                await animateSimulationStep(); // Introduce animation delay
                            }
                        
                        
                        
                        



                        } else if (algorithm === 'lifo') {
                            // LIFO algorithm logic
                            let reversedOrder = requestOrder.slice().reverse();
                            let currentPosition = initialPosition;
            
                            // Add initial position marker for LIFO algorithm
                            initialPositionMarker = [0, initialPosition];
            
                            for (const request of reversedOrder) {
                                if (simulationPaused) return;
                                const seekTime = Math.abs(request - currentPosition);
                                seekTimeArray.push(seekTime);
                                cylindersAccessedArray.push(request);
                                currentPosition = request;
            
                                // Remove the processed request from the array
                                requestOrder = requestOrder.filter(r => r !== request);
            
                                // Accumulate total initial movement
                                totalInitialMovement.lifo += seekTime;
            
                                await animateSimulationStep(); // Introduce animation delay
                            }
                        }
            
                        // Continue with the remaining logic for other algorithms if needed
                    }
            
                    async function animateSimulationStep() {
                        updateGraph(); // Update the graph with the latest data
                        updateTable(); // Update the table with the latest data
                        await sleep(simulationSpeed); // Introduce delay between animation steps
                    }
            
                    function updateTable() {
                        const dataTable = document.getElementById('dataTable');
                        dataTable.innerHTML = ''; // Clear previous table content
            
                        // Create table headers
                        const tableHeader = document.createElement('tr');
                        tableHeader.innerHTML = '<th>Step</th><th>Seek Time</th><th>Cylinder Accessed</th>';
                        dataTable.appendChild(tableHeader);
            
                        // Populate table rows with seek time and cylinders accessed data
                        for (let i = 0; i < seekTimeArray.length; i++) {
                            const tableRow = document.createElement('tr');
                            tableRow.innerHTML = `<td>${i + 1}</td><td>${seekTimeArray[i]} ms</td><td>${cylindersAccessedArray[i]}</td>`;
                            dataTable.appendChild(tableRow);
                        }
            
                        // Display average seek time
                        const averageSeekTime = calculateAverageSeekTime();
                        const averageRow = document.createElement('tr');
                        averageRow.innerHTML = `<td colspan="3" style="text-align: center;"><b>Average Seek Time: ${averageSeekTime} ms</b></td>`;
                        dataTable.appendChild(averageRow);
                    }
            
                    function calculateAverageSeekTime() {
                        const totalSeekTime = seekTimeArray.reduce((sum, seekTime) => sum + seekTime, 0);
                        return (totalSeekTime / seekTimeArray.length).toFixed(2);
                    }
            
                    function toggleSimulation() {
                        simulationPaused = !simulationPaused;
                        if (!simulationPaused) {
                            performSimulation(); // Resume the simulation if not paused
                        }
                    }
            
                    function sleep(ms) {
                        return new Promise(resolve => setTimeout(resolve, ms));
                    }
            
                    // Initial empty graph and table
                    updateGraph();
                   
                </script>

            </body>
            
            </html>            
           
