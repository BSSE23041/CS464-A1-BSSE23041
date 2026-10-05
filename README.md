# CS464 Assignment 01 · Fasiha Rohail · BSSE23041

## Game 1 · Pizza Ready

* **Store link:** https://play.google.com/store/apps/details?id=io.supercent.pizzaidle
* **Genre:** Idle / Tycoon Restaurant Simulator
* **I played:** 40 minutes, unlocked Counter, Drive-Thru, and hired 3 staff members
* **Video:** https://youtu.be/GZ8ec8a2fOg

<p>

<img src="Docs/game1/1.png" width="240">

<img src="Docs/game1/2.png" width="240">

<img src="Docs/game1/3.png" width="240">

</p>

1. **[M1, M2, M3, M5]** · The player is standing at the main counter and serving customers. The pizza stack is full and there is a $200 expansion tile nearby.

2. **[M6]** · The player is using the Table Upgrade station, which shows the speed and sale price upgrades.

3. **[M4, M7]** · An automated worker is serving customers at the pickup station, while cash is lying on the ground for the player to collect.

| #  | Mechanic                                                                        | Dynamic                                                                                                                                 | Aesthetic                                                                                             | Bartle type                                                                                           |
| -- | ------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| M1 | Virtual joystick movement with auto interaction on station overlap              | Players move around the store between the ovens, counters, and trash stations. They try to find the best route to keep working quickly. | Challenge: Players have to manage their movement and find efficient routes when there are many tasks. | Achiever: Players try to improve their routes so they can serve more pizzas in less time.             |
| M2 | Hard carry capacity limit ($N$ items max, upgraded with cash)                   | Players can only carry a certain number of pizzas. They have to decide when to deliver them or empty their stack.                       | Submission: This creates a simple and repetitive loop of collecting and delivering pizzas.            | Achiever: Players work on increasing their carrying capacity and improving their overall performance. |
| M3 | Dual window customer spawning queue (Counter & Drive-thru)                      | Players have to keep an eye on both the counter and drive-thru queues and move between them when one gets too long.                     | Challenge: Players have to decide which task to handle first when both queues need attention.         | Achiever: Players try to clear the queues and keep the store running smoothly.                        |
| M4 | On-ground cash drop and proximity pickup                                        | Players collect the money that appears on the floor while moving around the store. The money is then used for upgrades.                 | Sensation: Seeing and collecting the cash gives quick visual and audio feedback.                      | Achiever: Players collect money to increase their balance and buy more upgrades.                      |
| M5 | Pay to unlock expansion zones with cash threshold counters                      | Players save money and stand on marked tiles to unlock new parts of the restaurant.                                                     | Discovery: New areas, equipment, and customer types become available as the store expands.            | Explorer: Players are interested in seeing what new areas and features will unlock.                   |
| M6 | Exponential cost scaling per upgrade level ($Cost = Base \times Scale^{level}$) | Players decide whether to spend their money on speed, carrying capacity, or pizza price upgrades.                                       | Challenge: Players have to choose which upgrades will give them the best results.                     | Achiever: Players try to spend their money wisely and get the most benefit from each upgrade.         |
| M7 | Automated worker NPCs with upgradable speed and capacity parameters             | Players slowly move from doing all the work themselves to managing workers who handle different tasks.                                  | Fantasy: Players get the feeling of building and managing a growing restaurant business.              | Explorer: Players can watch the workers and see how the automated system works.                       |

**Aesthetic profile:** Submission, Fantasy, and Challenge. The game has a repetitive and relaxing loop of carrying pizzas and collecting cash. It also gives the player the feeling of building a business from the beginning. At the same time, players have to find good routes and choose useful upgrades.

**Player types**

* **Primary: Achiever (Acting × World)**, because 5 out of 7 mechanics (M1, M2, M3, M4, M6) focus on directly doing tasks in the game, increasing numbers, clearing customer queues, and earning more money.

* **Secondary: Explorer (Interacting × World)**, because M5 and M7 involve exploring the store, unlocking new areas, discovering new machines, and seeing how the workers perform different tasks.

---

## Game 2 · Apple Worm

* **Store link:** https://play.google.com/store/apps/details?id=com.icestonesoft.pavellotohov.appleworm.partners
* **Genre:** Grid Based Physics Logic Puzzle
* **I played:** 35 minutes, completed 7 levels
* **Video:** https://youtu.be/liJmh0vq8_Q

<p>

<img src="Docs/game2/1.png" width="240">

<img src="Docs/game2/2.png" width="240">

<img src="Docs/game2/3.png" width="240">

</p>

1. **[M1, M3]** · The worm is extending over a ledge while the unsupported parts of its body are affected by gravity.

2. **[M2, M4]** · The worm eats an apple and grows one segment longer. It can then use its longer body to cross a gap.

3. **[M6, M7]** · The worm moves past spike hazards and heads toward the exit portal.

| #  | Mechanic                                                                              | Dynamic                                                                                                                                | Aesthetic                                                                                                    | Bartle type                                                                                |
| -- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| M1 | Grid-based discrete step movement (1 cell per input key)                              | Players move one cell at a time, so they have to think about their moves before making them.                                           | Challenge: The game mainly tests planning and logical thinking instead of fast reactions.                    | Explorer: Players study the grid and try to understand how each move will affect the worm. |
| M2 | Snake body segment follow algorithm (Segment $i$ moves to cell of Segment $i-1$)      | Players bend and fold the worm's body to fit into small spaces and reach different areas.                                              | Discovery: Players learn how the worm's body behaves when it is folded into different shapes.                | Explorer: Players try different body shapes to see what they can do in tight spaces.       |
| M3 | Unsupported segment gravity check (Falls if zero underlying tile support)             | Players move the worm across gaps and have to make sure its body has enough support.                                                   | Discovery: Players learn how the gravity system works and what happens when part of the worm is unsupported. | Explorer: Players test different positions to understand where the worm can safely stay.   |
| M4 | Apple consumption growth trigger (+1 body segment upon entering apple cell)           | Players have to think about when and in what order to eat apples. A longer body can help cross gaps but can also make movement harder. | Challenge: The order in which apples are eaten affects how the rest of the puzzle can be solved.             | Achiever: Players try to collect the apples while completing the level.                    |
| M5 | Solid body collision and self-platforming (Segments act as physical barriers/bridges) | Players can place parts of their own body over gaps and use them as a platform to reach higher areas.                                  | Expression: Players can find different ways to use the worm's body to reach the target.                      | Explorer: Players look for new and creative ways to use the worm's body.                   |
| M6 | Instant death on hazard collision (Spikes trigger immediate level reset)              | Players can try risky moves and quickly restart the level if they fail. They then change their strategy.                               | Challenge: Players have to avoid the spikes and solve difficult sections through trial and error.            | Achiever: Players try to complete levels without hitting the hazards.                      |
| M7 | Exit portal level-complete trigger                                                    | Players move the worm's head into the exit portal to finish the level and move to the next one.                                        | Challenge: Reaching the portal gives the player a clear goal to complete.                                    | Achiever: Players complete levels one by one to progress through the game.                 |

**Aesthetic profile:** Challenge, Discovery, and Expression. The game focuses on solving spatial puzzles and avoiding hazards. Players also learn how gravity, growth, and the level layout work together. They can also find their own ways to use the worm's body to solve a level.

**Player types**

* **Primary: Explorer (Interacting × World)**, because M1, M2, M3, and M5 require players to interact with the game world and understand how the grid, body movement, gravity, and different physical situations work.

* **Secondary: Achiever (Acting × World)**, because M4, M6, and M7 give players clear goals such as collecting apples, avoiding hazards, reaching the exit, and moving to the next level.

---

## Level Blockouts

| Level   | Screenshot                                      | Its idea                                                                                                                             | Wayfinding tool                                                                                       |
| ------- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- |
| Level01 | <img src="Docs/levels/Level01.png" width="320"> | A simple straight stealth level that teaches basic movement, cheese collection, one Tom obstacle, and hiding behind cover.           | A straight cheese trail leads the player from the starting point to the exit door.                    |
| Level02 | <img src="Docs/levels/Level02.png" width="320"> | A loop-shaped level where the player has to collect all the food, deal with the noise carrots, and then return to the starting area. | Water puddles and vase hiding spots help show the player where the returning path goes.               |
| Level03 | <img src="Docs/levels/Level03.png" width="320"> | A winding level with two Tom hazards, red peppers that increase speed, and a guarded exit.                                           | Red pepper power-ups are placed at important points to help show the direction of the corridors.      |
| Level04 | <img src="Docs/levels/Level04.png" width="320"> | A 4-quadrant level that introduces three cat hazards, deadly black hole traps, and stair areas that can be used for hiding.          | The wall stairs and the corridors in the middle help guide the player between the different sections. |
| Level05 | <img src="Docs/levels/Level05.png" width="320"> | A level divided into 4 separate rooms. The rooms are connected through doorways, giving the player different ways to move and hide.  | The doorways between the walls show the player where they can move from one room to another.          |
