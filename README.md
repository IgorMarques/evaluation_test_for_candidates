# ZSSN (Zombie Survival Social Network)

## Problem Description

The world as we know has fallen into an apocalyptic scenario. A laboratory-made virus is transforming human beings and animal into zombies, hungry for fresh flesh.

You, as a zombie resistance member (and the last survivor who knows how to code), was charged on developing a system to share resources between non-infected humans.

## Features

You will need to develop a ***REST API***, which will store informations about the survivors, as well as the resources owned by them.

To do this, the api will need to have the following features:

- **Create users in the base**

  An user has *name*, *age*, *gender* and *last location (latitude, longitude)*.

  An user has an inventory of resources that he owns (empty at the time of creation).

  The accepted resources that can be in the inventory are: **water**, **food**, **aid kit** and **ammo**.

- **Update user location**

  An user must have the ability to update his last location, storing the new latitude/longitude pair in the base.

- **Flag a user as infected**

  In a chaotic situation like that, it's inevitable that an user gets contaminated by the virus.

  In this case, we need to flag an user as infected.

  An infected user cannot trade with other players, can't access his inventory, nor be listed in the reports (he is kinda dead anyway).

  **An user is marked as infected when at least three other users report his contamination.**

  When an user is infected, his inventory items are inaccessible.

- **Add/Remove items from inventory**

  An user can add/remove items from his inventory.

  The items that can be in the inventory are described above in the first feature.

- **Trade items**:

  Users can trade items with themselves.

  To do that, they must respect the price table below.

  Both sides of the trade should offer the same amount of points.

  You do not have to store the trade, but you must transfer the items.

| Item      | Points   |
|-----------|----------|
| 1 Water   | 4 points |
| 1 Food    | 3 points |
| 1 Aid Kit | 2 points |
| 1 Ammo    | 1 points |

- **Reports**

  You need to be able to generate these reports using the api:
    1. Percentage of infected users.
    1. Percentage of non-infected users.
    3. Mean quantity of each kind of resource by user (e.g. 5 waters per user)
    4. Points lost by infected users.

---------------------------------------

1. Use any programming language or framework, choice is yours;
2. No authentication is needed (it's a zombie apocalypse, no one will try to hack a system while running from a horde of zombies);

**GOOD LUCK**
