# ZSSN (Zombie Survival Social Network)

## Problem Description

The world as we know it has fallen into an apocalyptic scenario. A laboratory-made virus is transforming human beings and animals into zombies, hungry for fresh flesh.

You, as a zombie resistance member (and the last survivor who knows how to code), was charged to develop a system to share resources between non-infected humans.

## Features

You will need to develop a ***REST API*** (yes, we care about architecture design even in the midst of a zombie apocalypse!), which will store information about the survivors, as well as the resources they own.

To do this, the api will need to have the following features:

- **Create users in the database**

  An user has to have *name*, *age*, *gender* and *last location (latitude, longitude)*.

  An user has an inventory of resources of his own property (which you need to declare at the initial registration of the user).

  The only kinds of resources that can be in the inventory are: **water**, **food**, **medication** and **ammunition**.

- **Update user location**

  An user must have the ability to update his last location, storing the new latitude/longitude pair in the base (no need to track locations, just replacing the previous one is enough).

- **Flag user as infected**

  In a chaotic situation like that, it's inevitable that an user gets contaminated by the virus.

  In this case, we need to flag an user as infected.

  An infected user cannot trade with other players, can't access his inventory, nor be listed in the reports (he is kinda dead anyway, see the item on reports below).

  **An user is marked as infected when at least three other users report his contamination.**

  When an user is infected, his inventory items are inaccessible (he cannot trade with other users).

- **Users cannot Add/Remove items from inventory**

  His belongings must be declared when he is first registered in the system, then he can only change his inventory by means of trading with other users.

  The items that can be in the inventory are described above in the first feature.

- **Trade items**:

  Users can trade items among themselves.

  To do that, they must respect the price table below. The currency is just "points" of value of the items.

  Both sides of the trade should offer the same amount of points. For example, 1 Water and 1 Medication (1 x 4 + 1 x 2) is worth 6 ammunition (6 x 1) or 2 Food items (2 x 3).

  You do not have to store the trade transaction, but you must transfer the items between the users.

| Item         | Points   |
|--------------|----------|
| 1 Water      | 4 points |
| 1 Food       | 3 points |
| 1 Medication | 2 points |
| 1 Ammunition | 1 points |

- **Reports**

  You need to be able to generate the following reports using an API endpoint:

    1. Percentage of infected users.
    1. Percentage of non-infected users.
    3. Average quantity of each kind of resource by user (e.g. 5 waters per user)
    4. Points lost because of infected users.

---------------------------------------

1. Use any programming language or framework, the choice is yours;
2. No authentication is needed (it's a zombie apocalypse, no one will try to hack a system while running from a horde of zombies);
3. We still care about proper programming and architecture techniques, you must showcase that you're worthy of surving the zombie apocalypse through the sheer strength of your skills;
4. Don't forget to make at least a minimal documentation of the API endpoints and how to use them;
5. From the problem description above you can do a very bare bone solution or you can add optional features that are not described. Use your time wisely - the best possible solution might just take too long to be effective in the apocalypse - so you must do the best possible solution that will hold up within the least ammount of time and still be able to showcase your skills in order to prove your worth.

**ARE YOU NEGAN?**
