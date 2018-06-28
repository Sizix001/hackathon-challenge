Teamleader Hackathon
====================

Meatdealer
----------

You are one of founders of a startup called Meatdealer. Meatdealer has found a brilliant way to grow tasty synthetic meat, in a state of the art laboratory.

Last week, at a vegetarian conference, we managed to gather a list of over a 100 companies that are interested in distributing our animal friendly meat.

We currently have 2 sales representatives with jet-packs. Yes, real jet-packs. With these, they can travel from meeting to meeting in a straight line at a constant speed of 60 km/h. Once they arrive, it takes them exactly 45 minutes to potentially close the deal. These guys are amazing!

The Challenge
-------------

The next week is crucial for the success of Meatdealer. You, the mastermind behind Meatdealer, are asked to optimize next week's working schedule for both of our sales representatives.

You can find a csv of interested companies [https://github.com/teamleadercrm/hackathon-challenge/blob/master/input.csv](here). And it looks like this:

```csv
Id,Value,Probability,Latitude,Longitude,"Preferred Weekday"
1,97760,0.68,49.06578,2.88862,tuesday
2,38762,0.93,48.7841,1.89458,wednesday
3,88848,0.4,49.02375,2.21236,tuesday
4,87469,0.12,48.41628,2.33924,tuesday
5,32441,0.56,49.10262,2.53774,tuesday
```

In this file, you will find the following information:

- A deal identifier
- The deal value (in €)
- The probability to close the deal (between 0 and 1)
- The latitude and longitude, specifying the lead's location
- The potential lead's preferred weekday to be visited (see bonus)

At Meatdealer, we work hard and play hard. Our sales representatives work 8 hours a day (not a single minute longer). They always start the day at the office, and must be back by the end of the day to celebrate their closed deals with beers and synthetic pepperoni pizzas.

The Meatdealer office is at WeWork Coeur Marais. The jet-pack coordinates are:

- Latitude: 48.861804
- Longitude: 2.359132

It all depends on you. Compared to synthetic meat, this should be easy. The expected csv output of your algorithm should look like this:

```csv
0,0,23
0,1,49
0,2,76
1,0,47
1,1,42
1,2,12
```

With these columns respectively:

- The number of the salesperson (zero based)
- The day of the week (zero based, with Monday as the start of the week)
- The identifier of the deal (found in the input file)

Make sure that the meetings in your output are a chronological order.

We will evaluate your solution based on the cumulative weighted revenue (probability * value) of your working schedule. The person/team with the highest total weighted revenue wins!

Once you have a working schedule, you can upload it at [https://paris-hackathon.teamleader.eu](paris-hackathon.teamleader.eu). You can upload as many times as you want. And remember, a sub-optimal working schedule is better than no schedule.

Good luck!

Bonus
-----

Every lead has a preferred day of the week on which he would like to be contacted by our sales representative. If the sales representative visits the lead on that day, the probability of closing the deal increases by 10%. Keep in mind that the probability can not be higher than 100%.
