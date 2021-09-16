---
subpage: false
title: Venn Diagram of Me
hide:
- toc
weight: 1
tags: 
- Module1
- RGB color model
- Processing
---

{{< columns >}} 

## Goal:

Use the RGB color model to create a Venn Diagram that showcases your personality.

<img src="/images/recipes/logicalDot.png" height="400" alt="meme image">
<---> <!-- separator between columns -->

## Steps:
1. Find the Venn Diagram recipe program ( VennDiagram.pde ) and open it using Processing.
2. Run the program and you should see an empty gray window.
3. After the size() command, add code to draw 3 circles to form a Venn Diagram (see picture). The command to draw a circle in Processing is:
	````
	ellipse (centerX, centerY, circleWidth, circleHeight);

	````
4. Change the x and y of each ellipse until they overlap as in the picture.
5. Run the program. It should look a bit like this
<img src="/images/recipes/whiteCircles.png" height="300">
6. Now to add the colors. Processing uses the following command to draw in color
	````
	fill(red, green, blue, opacity);

	````
	where red, green, blue, and opacity are all numbers between 0 and 255. So to make see-through red circles, we add the following line of code BEFORE we draw the circles.
	````
	fill(255, 0, 0, 100);

	````
7. Run the program. It should look a bit like this
<img src="/images/recipes/redCircles.png" height="300"> 
	We can now see the edges of all the circles because we made them "see-through" by setting the opacity to 100 (which is < 255)

8. Add more fill commands (you will have to figure out where to put them) so that each ellipse has its own unique color.
	
<img src="/images/recipes/colorfulCircles.png" height="300">

9. Label each of the circles with an aspect of your personality. Processing uses the following command to draw text. You will need to put numbers in place of xLocation, and yLocation. Play around with the x and y until it works with your diagram.

	````
	text("TEXT", xLocation, yLocation);

	````

10. You can also make the text larger by changing the sizeOfLetters (you will have to figure out where to put this)


	````
	textSize(sizeOfLetters);

	````


  <a href="https://processing.org/reference">
    <img src="/images/p3logo.jpeg" height="100" class="footer" alt="Processing Reference"></a>

{{< /columns >}}
                    