# This is the Title

## sub bullet
- line one email
    - whaat it do
w;lf;oewj rovqpr2qpr

>[!WARNING]
>This is a demo


# studentwtcc-github.io
1. Your name and email address
2. A brief description of your Github account
3. A brief description of the repository you created
4. A brief description of the steps you took to clone the repository onto your local machine

```python
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="https://pyscript.net/latest/pyscript.css" />
    <script defer src="https://pyscript.net/latest/pyscript.js"></script>
    <title>Number Guessing Game</title>
    <style>
        label {
            display: block;
        }
    </style>
</head>
<body>
    <py-config>
        packages = ["numpy"]
    </py-config>
    <py-script>
        import numpy as np
        selection = np.random.randint(0, 100, 1)[0]
    </py-script>

    <form>
        <label for="guess">Guess:</label>
        <input name="guess" id="guess">

        <button type="button" id="submit">Check Guess</button>
        <label for="result">Result:</label>
        <div name="result" id="result"></div>    
    </form>

    <py-script>
        from pyscript import when
        
        @when("click", selector="#submit")
        def check_guess():
            user_guess = int(Element("guess").value)
            result = Element("result")
            if user_guess == selection:
                result.write("Congratulations! You guessed correctly.")
            elif user_guess > selection:
                result.write("Try again! Your guess was too high.")
            else:
                result.write("Try again! Your guess was too low.")
    </py-script>
</body>
</html>
```
```python
# Simple Python program to greet the user and calculate their age in 5 years

# Ask for the user's name
name = input("What is your name? ")

# Ask for the user's age
age = int(input("How old are you? "))

# Calculate the age in 5 years
age_in_5_years = age + 5

# Print the personalized message
print(f"Hello, {name}! In 5 years, you will be {age_in_5_years} years old.")
```
