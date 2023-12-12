<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Number Guessing Game</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 50px;
    }
  </style>
</head>
<body>

  <h1>Number Guessing Game</h1>
  <p>Guess a number between 1 and 10:</p>
  <input type="number" id="userGuess">
  <button onclick="checkGuess()">Submit Guess</button>
  <p id="result"></p>

  <script>
    // Generate a random number between 1 and 10
    const secretNumber = Math.floor(Math.random() * 10) + 1;

    function checkGuess() {
      // Get the user's guess from the input field
      const userGuess = parseInt(document.getElementById('userGuess').value);

      // Check if the guess is correct
      if (userGuess === secretNumber) {
        document.getElementById('result').innerText = 'Congratulations! You guessed the correct number!';
      } else {
        document.getElementById('result').innerText = 'Sorry, try again!';
      }
    }
  </script>

</body>
</html>

--->
