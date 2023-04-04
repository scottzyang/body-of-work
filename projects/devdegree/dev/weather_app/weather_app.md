## Weather App - DEV
*Weather App* is a command-line program written in JavaScript and utilizes the [OpenWeather API](https://openweathermap.org/api) to receive real-time weather-related data based on user input. This program served as the final group project to end the DEV curriculum as part of the Training Path.

Example: User inputs "Minneapolis" as location.

<img src="weather_app.png" width=500>

### Links
- [WeatherApp Repository](https://github.com/DevDegree/weather-app) (Internal to Shopify/DevDegree Only)

### Noteworthy Responsibilities
- Develop the `while` loop within logic flow within the `main.js` file to handle user selected options.
- Develop the `comparecities` helper function to input two cities and compare weather data received from OpenWeather API. Also handled the celsius and fahrenheight temperature conversation integration into `comparecities` function.
- Create the `displayWeather()` method within the `weatherClass` file and debug associating issues. The display method shows the city weather data and needed to display either `Fahrenheit` or `Celsius` depending on the user input.
- Debugged start-up logic to exit program
- Troubleshoot merge conflicts between group members.

### Learning/Outcomes
- Biggest learning we had throughout this group project actually had nothing to do with coding itself. We constantly ran into `merge conflicts` with our work, and struggled with managing working branches. None of us had any experience working in a group before, and we had to practice open communication whenever anyone made changes to main. Through this we also learned a lot about `git rebase`, which essentially takes in the most updated version from the remote repo and adds your current local changes on top of it. This was a super neat trick to learn.
- DEBUGGIN. We had a lot of issues with our program not working correctly.
- Learned about ANSI Code and how it can be used to change the color of the terminal text. For instance this code block here: `tempColor = '\u001b{34m${this.temp.toFixed()}}\u001b[0m'`.
  >`\u001b{34m` is the ANSI code for Blue, therefore it will change the text color to Blue.

  >`\u001b[0m` is the ANSI code for Reset, therefore it will reset the text color back to normal.

  Wrapping the `this.temp.toFixed()` in the `\u001b{34m....\u001b[0m` will set the text between it to Blue, then reset it right after. Neat little trick to change the color of the temperature according to the temperature (view image above for blue 3&deg;C).
- Big fan of using [`ternary operators`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator) to handle simple display logic. For instance, `${cityOne.temp.toFixed()}${!isInCelsius ? '°F' : '°C'}`.
  > `cityOne.temp.toFixed()` simply displays the temperature value (i.e 45)

  > `!isInCelsius ? '°F' : '°C'` is the ternary operator.

  Based on the value of `isCelsius` it'll either display `°F` or `°C`. Ternary operators allowed us to have nice, inline, and clean code.

- Thanks to a group mate I learned a lot about `async await` and how to make requests to an API. Still not 100% on understanding this, but, from what I know, we use this to run code while we await a response from an API.

### Reflection
- This group assignment was super fun, although we had a lot of issues with merge conflicts, everyone was super graceful in handling errors and mistakes. I was super uneasy going into this group project just because I often lack confidence in my knowledge and skill, but everyone was super reassuring and took time to be receptive to questions. I'm proud of myself for speaking out when I didn't understand something, for instance the `async await` was completely new to me and I also never worked with APIs before. Before I probably would've just stayed silent in my lack of knowledge, but I made sure to ask questions to understand. Overall it was a great experience, even the hiccups were a great learning experience. Looking forward to more group projects going forward.
