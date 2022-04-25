This project encapsulates a quick trip to the casino! You start with R$1000 and can choose to bet either the maximum or minimum amount. You then pull the reel, are notified if you won or lost, and watch as your credit either increases or decreases.
 
Link: https://casino-copacabana.netlify.app/
 
![rio](https://user-images.githubusercontent.com/98935149/164952110-e5f16dea-d0c9-485e-b8bf-423c711733a0.jpg)
 
How?
Tech: HTML, CSS, JS
HTML: 
I first created an h1 for the most important heading on the platform, followed by a section with three p elements, each of which stands for a reel. Below that I have a div element with three button elements. These buttons each have a value of “button” assigned to the attribute of “type”. Lastly, I included a div element which includes the h2 element in which “Won!” or “Lost!” are added following each round.  Next, the amount bet by the user, the score board, and a note which states the currency being used. 
CSS:
The styling sheet includes text being centered by assigning the property value ”center” to the property “text-align”, as well as headings and other pieces of text being assigned font sizes and font weights. Flexbox is used to line up the buttons and reels, and the “line-height” property is used to place the text in the center of its container, top to bottom. Borders are assigned to several things to make them stand out in front of the body’s background image. Some items’ edges are rounded using the property “border-radius”. Min- and max- width are assigned to several items to ensure that they don’t shrink or expand too much as screen size increases
 or decreases. 
JS:
First, variables are declared and assigned values of elements in the Dom in order to make them easier to manipulate. The three buttons are given event listeners, all of which are triggered with clicks. The two buttons used for betting, Maximum Bet and Minimum Bet are assigned the same function, betting, while the remaining button, Feeling Lucky?,  is assigned the function spin. spin first  assigns an empty string to the inner text of the h2, which is set to hold the outcome of each round. It then calls the same function three times, once per reel. This function uses the random method to randomly come up with a number (between 0 and 0.999) five times. There is a conditional that states that if each of these numbers falls within a certain range, it is assigned to a number between 100 and 500, which are the numbers which are shown on the reel. Below the three function calls in spin are two more function calls. The first takes the inner text of the three reels as parameters, comparing them in order to determine whether the user has won or lost. The latter simply calls a function without parameters but with a conditional that determines whether the word “Win” or “Lost” is added to the designated placeholder.
 
Optimizations: The first time I got the reel to run, I had set up three different functions for each reel. This made my code more complex and far harder to read. I went back and called a function three times inside of an event listener’s function, which ran the same function three times without having to code everything out three times. 

Lessons Learned: 
This was the first time I called a function three times within another function to come up with three different results. I practiced this newly-acquired method by deleting my code and rewriting it continuously. I did this while reading each line out loud in hopes of retaining the technique. I enjoyed learning this and absolutely love how Javascript is a combination of language and analytical thinking. 

