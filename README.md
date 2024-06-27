Auction System
This is a simple C++ auction system where participants can place bids on paintings. The highest bid wins the painting.

Features
Participants: Add participants to the auction with their details (name, age, gender, and id).
Paintings: Add paintings to be auctioned with their names and minimum bid amounts.
Bidding Process: Conduct the auction by allowing participants to place bids on the paintings.
Winner Determination: Determine the highest bidder for each painting and announce the winner.
Classes
Participant
Represents a participant in the auction.

Attributes
name (string): The name of the participant.
age (int): The age of the participant.
gender (char): The gender of the participant ('M' or 'F').
id (int): The unique ID of the participant.
Methods
get_name(): Returns the name of the participant.
get_id(): Returns the ID of the participant.
Painting
Represents a painting to be auctioned.

Attributes
name (string): The name of the painting.
minimum_bid (int): The minimum bid amount required for the painting.
highest_bidder (Participant*): The participant who placed the highest bid.
highest_bid (int): The highest bid amount.
Methods
get_name(): Returns the name of the painting.
get_minimum_bid(): Returns the minimum bid amount.
get_highest_bidder(): Returns the highest bidder.
get_highest_bid(): Returns the highest bid amount.
place_bid(Participant* bidder, int bid_amount): Places a bid for the painting.
Auction
Manages the auction process.

Attributes
participants (vector<Participant*>): A list of participants in the auction.
paintings (vector<Painting*>): A list of paintings to be auctioned.
Methods
add_participant(Participant* participant): Adds a participant to the auction.
add_painting(Painting* painting): Adds a painting to be auctioned.
conduct_auction(): Conducts the auction and determines the highest bidder for each painting.
Usage
To run the auction system, follow these steps:

Add participants to the auction.
Add paintings to be auctioned.
Conduct the auction.
