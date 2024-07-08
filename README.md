<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Search Interface</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Arial&display=swap');
        body {
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #ADD8E6; /* Light blue background */
        }
        .search-container {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .search-container h1 {
            margin-bottom: 20px;
            font-size: 24px;
        }
        .search-container .search-bar {
            display: flex;
            gap: 10px;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
        }
        .search-container select,
        .search-container input[type="text"],
        .search-container button {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }
        .search-container select {
            background-color: #fff;
        }
        .search-container input[type="text"] {
            flex-grow: 1;
        }
        .search-container button {
            background-color: #4CAF50;
            color: white;
            cursor: pointer;
            border: none;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .search-container button:hover {
            background-color: #45a049;
        }
        .search-container button:before {
            content: "\1F50D"; /* Unicode for search icon */
            position: absolute;
            right: 15px;
            font-size: 20px;
        }
    </style>
</head>
<body>

  <div class="search-container">
        <h1 style="font-weight: 600;">P E S INSTITUTION</h1>
        <div class="search-bar">
            <select name="categories" id="categories">
                <option value="everything">Everything</option>
                <option value="software-development">Software Development</option>
                <option value="web-development">Web Development</option>
                <option value="data-analyst">Data Analyst</option>
                <option value="it-consultant">IT Consultant</option>
                <option value="network-administrator">Network Administrator</option>
            </select>
            <input type="text" id="search" name="search" placeholder="Search anything">
            <button type="button">Search</button>
        </div>
    </div>

</body>
</html>
