# Self-Evaluation: Emoji Vacation

## Checklist

### Correctness

- [x] Image background shows trees 60% of the time, and mountains 50% of the time (mountains and trees may both appear in one image)
- [x] The program draws a “family” of emojis, containing a number of emojis based on the parameters to `createFamily()`
- [x] Each emoji in the family is randomly selected, based on your implementation of `createRandomEmoji()`
- [x] When run, your program iterates through an endless slideshow of these emoji photos, each with randomized backgrounds and emoji styles
  - [x] There is a pause for three seconds on each image so that a viewer may enjoy the slideshow!
- [ ] (Optional) Additional randomly-selected background scenery
- [x] (Optional) A dark transition between each slide of the slideshow
- [ ] (Optional) Child and adult emojis are shown in a random order
- [ ] (Optional) Modify the background to include multiple times of day in the random scenery

### Code Style

Check these items from the [Comp 127 Style Guide](https://comp127.innig.net/resources/style-guide/):

- [x] all classes are in packages
- [x] package names start with a lowercase letter
- [x] newly created Java files have a header comment with
    - [x] author name
    - [x] brief description of class, and
    - [x] acknowledgement, if appropriate
- [x] identifier (variable and method) names are descriptive
- [x] variable and method names are in lowerCamelCase (no CapitalizedNames,
  names_with_underscores)
- [x] class names are singular nouns
- [x] class names are in UpperCamelCase
- [x] proper indentation:
    - [x] opening curly braces (“{”) are at the end of the line
    - [x] closing curly braces (“}”) are on their own line
    - [x] the indentation of closing braces is the same as the indentation of the
      opening statements they match
    - [x] lines are indented according to how deeply they are nested
- [x] completed TODOs are deleted
- [x] extra blank lines are deleted
- [x] unneeded commented lines of code are deleted
- [x] print statements used for testing are deleted


## Reflection

Briefly reflect in writing on your experience solving this exercise. Just a
sentence or two in response to each question is plenty.

**What did you miss? What did you wish you did better?**

One thing I missed was a pesky + instead of a - in my code for positionFamily(). What I wish I did better in that case was actually pay attention to how CanvasWindows actually work before barging in and trying to use them. (It took me absolutely forever for me to realize that increasing y position goes down. Which is even funnier because I'm already used to an environment where that's the default anyway.)

**What challenges did you face, and how did you overcome them?**

Really, the biggest challenge was just that sign flip, honestly. How I eventually overcame it was by reducing the number of variables that were affecting the result. I got rid of compensating for the size of the emojis, and I realized what happened when they went _up_ instead of down.

**What is something that was interesting or exciting, or a lesson you learned from this experience that you want to remember?**

One thing I found really exciting was that evidently KiltGraphics lets you make a triangle with arbitrary vertices (seen in the mountains), because that means you can do 3D rendering.