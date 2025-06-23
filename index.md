<!--
# Wrist Rehabilitation Device
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!
You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
This is an HTML comment in Markdown
Anything between these symbols will not render on the published site
```
-->
| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Jas S | Basis Independent Fremont | Mechanical Engineering | Incoming Junior
<!---
**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**
-->
(JasnoorS.HEIC)
<!---
# Final Milestone


**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/y3VAmNlER5Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
Challenges:
While I was trying to install bluetooth, an issue arose where the sensor would disconnect itself after 5 seconds. To solve this I decided to transfer over to using Adafruit IO which is a website. To do this I required a wifi connection and to set up the data receving on the website. However, there was a data rate limit.
For your second milestone, explain what you've worked on since your previous milestone. You can highlight:
- Technical details of what you've accomplished and how they contribute to the final goal
- What has been surprising about the project so far
- Previous challenges you faced that you overcame
- What needs to be completed before your final milestone 
-->
# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/fmthsALyXC0?si=sA5ARxU7Pw9Ax2rS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

My First milestone was to be able to accurately receive data fromt he flex sensor with a high accuracy. For example, I had to find the angle of the bend in the flex sensor:
(FlexCircuit)

Description:
So far, I've understood how the flex sensor works and how the accelrometer works. However, I've only identified how to use the flex sensor and receive an accurate angle. To do that I plotted the data I received from bending the flex sensor at a certain angle. Below is the function that I created from the data:
Graph:
(Graph)
y1 = m * (a * x1 - b) + c1 * cos(f1 * x1 + p1)+ c2 * cos(f2 * x1 + p2) + c3 * cos(f3 * x1 + p3) + c4 * cos(f4 * x4 + p4) + c5 * cos(f5 * x1 + p5) + c6 * cos(f6 * x1 + p6) + c7 * cos(f7 * x1 + p7) + c8 * cos(f8 * x1 + p8)
I used this equation so that the graph was fit to my data very tightly. This makes it so that I have a 99.85% accuracy relative to my data. This means that it isn't 99.85% accurate to the actual angle but the angles that I measured instead. I did this because I was pretty confident with my measurements as I took around 50 measurements.

Challenges:
Some challenges I faced were identifying how to make an equation that matches it. Once I learned about using C * cos (f * x + p) I added more until the acccuracy reached its highest. Another challenge I faced was when taking measurements, the sensor would return values that don't make any sense that are way too high ot low. To solve this, I took many measurements and averaged them. I also had taken the average of the last ten valeus when actually writing the code to exclude outliers and make it more accurate.

Next Steps:
Next, I want to find a way to use the accelerometer and then transfer the data from both sensors by bluetooth.


# Starter Project - Retro Arcade Console

<iframe width="560" height="315" src="https://www.youtube.com/embed/HoTiaGMx5EQ?si=7KrHkXm_49cLGxsC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Description:
In the starter project, I created a retro arcade console. First, I soldered on the LED displays which would be the screen and score display. Then, I soldered the USB port to be able to change the data in the microcontroller. Then, I soldered on the buttons for input. Next I attached the battery pack to the back case, trimmed the wires, and attached the wires to allow for power. I added the capicator and cut off the extra metal since it stuck out very far. The switch was placed between the power and the rest of the circuit to be able ot turn the power on and off. Finally, I added a vibrator to add a new effect. When creating this project I learn't how to sauter, desauter, and splice wires.

Challenges:
My biggest challenges were that I had to restart the starter project twice. The first time I accidently melted the switch with the soldering gun while working on soldering the wires. The switch was already solered on the board and wouldn't budge even after desoldering. The second time I had placed the displays upside down and so the polarity of the displays got messed up. The displays also wouldn't get desoldered after an hour of trying. On the third attempt, I finally finished the project.

Next Steps:
My next steps will be to understand how the parts for my main project work and how I can use them to make my wrist rehabilitation device. Then, I will have to find a way to accuratly measure the angle of the device
<!--
# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
-->
