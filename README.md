**Teamleader hackathon**



Meatdealer has 2 sales representatives. They start at the office (coördinates below) and like to be back within their 8 hour working day. It takes them 45 minutes to close a deal. Every time again! Oh, and they have jetpacks! Yes, real jetpacks! They won't tell where they got them, but all we know is that they definitely travel in straight lines at 60km/h, constantly!

Our marketing team gathered some really good clients and put them all into a nice csv list! Every line has, in that order:

- A deal identifier
- The deal value (in €)
- The probability to close the deal (between 0 and 1)
- The latitude &amp; longitude, specifying the lead&#39;s location
- The potential client&#39;s preferred weekday to be visited.


Example:

![Input Format](/input.png)

Anything else we need to add? Well, yes: our office address (Teamleader Paris):
- Latitude: 48.861804
- Longitude: 2.359132

You are asked to make a software tool to plan a week schedule for the two sales representatives that plans meetings with the customers that results in the highest weighted (probability \* value) revenue possible.

The solution with the highest combined revenue wins.

_Bonus: the deal probability is increased by 10% if you visit the lead on the prefered day of the week! Keep in mind, the probability can not be higher than 100%._

You can upload your solution to our submission website (https://paris-hackathon.teamleader.eu). Please do so in the following format:

![Output Format](/output.png)
 
Where the numbers are respectively:

- The number of the salesperson
- The day of the week
- The identifier of the deal

Separate by a semi-colon, no header row and you&#39;re good to go!

Obviously, sort them in the same order you want your sales representative to visit them.

Upload your solution at [https://paris-hackthon.teamleader.eu](https://paris-hackthon.teamleader.eu) and cross your fingers!

Good luck!
