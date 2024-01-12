# Exercise Link: <br>
https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Test_your_skills:_Events#events_1<br>

# Instructions:<br>
Now we'll look at keyboard events. To pass this assessment you need to build an event handler that<br>
moves the circle around the provided canvas when the WASD keys are pressed on the keyboard. <br>
The circle is drawn with the function `drawCircle()`, which takes the following parameters as inputs:<br>

`x` — the x coordinate of the circle.<br>
`y` — the y coordinate of the circle.<br>
`size` — the radius of the circle.<br>

# My Solution:<br>
```
// Add your code here
      const moveCircle = (event) => {
        let keys = event.key.toLowerCase();
        switch (keys) {
          case "w":
            drawCircle(400, y, 30);
            break;
          case "a":
            drawCircle(400, 250, 30);
            break;
          case "s":
            drawCircle(50, 250, 30);
            break;
          case "d":
            drawCircle(50, 50, 30);
            break;
          default:
            console(`${key}`);
            break;
        }
      };

      document.addEventListener("keypress", moveCircle);
```


