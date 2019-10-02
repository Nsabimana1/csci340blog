---
layout: post
title:  "Data Modeling"
date:   2019-10-01
---

**Description**

An auction website has items for sale that are provided by sellers. Each item has an opening price, a description, and an ending time. Customers submit bids. The highest, earliest bid submitted before the ending time is the winning bid and the item is sold to the bidder. Each seller must pay the auction company 5% of the winning bid. The auction company wants to be able to analyze the sales behavior of its customers and sellers and so must keep track of all bids and sales.

**Used tables**
- User
- Auction
- Bid
- Purchase
- Item


**Assumption**

In order to model this scenario  into a database schema, I made the following Assumption:

The user table will store the recorders of all users, and each user can ether be a buyer or a seller. That distinction is kept in privilege column of User table. In addition, I assumed that the seller will list a product as an auction, which is an item in this case, and other people will send the bids for that auction. The buyers will keep bidding until the ending time of the bid.

After the ending time of an item, the buyer with the highest bid will Purchase the item. This Information will be recorded in the Purchase table.
When the auction company is looking for the way to charge 5% of the Purchase, it will look for each Purchase, get an auction id number associated with it and a bid id number associated with it and use that information to deduct 5% of the money payed on the highest bid from the item's seller associated with that auction.

**Bellow is the Entity Relation Diagram from Draw.io**
<img src="{{ '/assets/img/CSI 340 lab5.png' | prepend: site.baseurl }}" alt="">

**Bellow is the Entity Relation Diagram of a Database Schema from Vertabelo**
<img src="{{ '/assets/img/Auction_Management_System-2019-10-01_22_11.png' | prepend: site.baseurl }}" alt="">

I am satisfied with my resulting data representation.
