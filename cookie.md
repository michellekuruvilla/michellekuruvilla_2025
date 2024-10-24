---
layout: base
title: Course Descriptions
description: An overview of Computer Science pathway at Del Norte High School
permalink: /cookie/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Super Cute Cookie Clicker</title>
    <style>
        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            background-color: #f0e4d7;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        .game-container {
            margin-top: 50px;
        }

        h1 {
            color: #a0522d;
        }

        .cookie {
            width: 200px;
            height: 200px;
            background-color: #d2b48c;
            border-radius: 50%;
            margin: 0 auto;
            position: relative;
            cursor: pointer;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }

        .cookie::before, .cookie::after {
            content: '';
            position: absolute;
            background-color: #8b4513;
            border-radius: 50%;
        }

        .cookie::before {
            width: 30px;
            height: 30px;
            top: 40px;
            left: 60px;
        }

        .cookie::after {
            width: 25px;
            height: 25px;
            top: 100px;
            left: 120px;
        }

        .cookie .chocolate-chip {
            width: 20px;
            height: 20px;
            background-color: #8b4513;
            border-radius: 50%;
            position: absolute;
        }

        .cookie .chocolate-chip:nth-child(1) {
            top: 30px;
            left: 120px;
        }

        .cookie .chocolate-chip:nth-child(2) {
            top: 90px;
            left: 50px;
        }

        .cookie .chocolate-chip:nth-child(3) {
            top: 130px;
            left: 90px;
        }

        p {
            font-size: 1.5rem;
            color: #8b4513;
        }
    </style>
</head>
<body>
    <div class="game-container">
        <h1>Super Cute Cookie Clicker!</h1>
        <div class="cookie" id="cookie">
            <div class="chocolate-chip"></div>
            <div class="chocolate-chip"></div>
            <div class="chocolate-chip"></div>
        </div>
        <p>Cookies clicked: <span id="counter">0</span></p>
    </div>

    <script>
        let counter = 0;
        const cookie = document.getElementById('cookie');
        const counterDisplay = document.getElementById('counter');

        cookie.addEventListener('click', function(e) {
            // Check if the clicked element is the cookie itself, not a chocolate chip
            if (e.target.id === 'cookie') {
                counter++;
                counterDisplay.textContent = counter;
            }
        });
    </script>
</body>
</html>


