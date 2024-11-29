# GameProject

![Banner](images/collab.png)

Name - A top down grid turn based RPG style game with characters to use and enemies to fight with a turn system using a FI/FO organization method. Battles include physical attacks, magical attacks and more. Battle animations and sprites included to display characters to use and enemies to fight.


## ✒️ Description

In this turn-based battle game, users fight using playable characters to attack enemies on the field using physical or magical attacks to reduce all enemies healths to 0 until all enemies or all allies die. Characters and enemies fight on a grid style battleground and can only move within a certain range around where they are.

## 🕹️ Gameplay

The game starts with the turn order being randomized and allies are at the bottom right of the field and enemies are at the top left, the first entity at the top of the turn order goes, if its an enemy, they choose between a magic attack or physical attack and they do that. If it was an ally, the battle menu state pops up and you can choose which option you want to do, attack, magic, item or run which then proceeds to do different things. 

Attack will put a selector above an enemy with the choice to switch between enemies and until you press a button, the enemy will be highlighted and you can see a display showing their health and other info. If you press attack then you will move to the grid spot closest to the enemy along your path to do a physical attack that will knock them back. 

If you choose magic, you can see a casting animation playing while your magic attack will happen on a later turn as shown in the turn order bar. When you're choosing the enemy to attack with it, you see the enemy info just like when you choose attack. When the magic turn happens the ally casts the spell and does damage to the enemy chosen and then gets pushed further down the turn order.

If you choose item, you will see a list of items you currently have and can use and if an item is selected you will have the selector over yourself initially but you can move it around on your allies for the desired effect the item has when used. 

If the run option is chosen, the characters will fade out and a text box will have said that you successfully ran.

After each entity's turn has went, they move down the turn order bar a certain amount to then let the next entity attack. The turn order bar is infinite and battles don't end until one group is all dead or player has run.

## 🧱 Features

-   **Combat Grid** Entities have a 2D grid to move around on. There may be blocks or objects in the way during battle.
-   **Combat Menu** Users have a Combat Menu to select options from during battle to allow them to do actions included in the menu.
-   **Movement** Users can move a character around the Combat Grid using the move selection in the Combat Menu.
-   **Attack** Users can select Attack on the Combat Grid to attack an enemy with a physical attack within a range around the character to deal damage to the enemy's health.
-   **Magic** Users can select Magic on the Combat Grid to attack an enemy with a magical attack with an unlimited range to deal damage to the enemy's health.
-   **Items** Users can select Item on the Combat Grid to use an item on a popup screen with all the items they may be holding that can heal the user or do other functions.
-   **Run** Users can select Run on the Combat Grid to run away from a fight.
-   **Character Information Profiles** Users can view the Health Points and Magic Points of a character at the bottom of the screen.
-   **Turn Order Bar** Users can view the turn order of characters and enemies on a bar on the left of the screen with the next characters being the ones near the top and the last being the ones at the bottoms.
-   **Enemy Information** Users can view information about the enemy while hovering over an enemy with an attack selector or magic selector.

#### User Combat Stories

-   As a user, I want to move a certain distance within the range I have.
-   As a user, I want to move and attack in one turn.
-   As a user, I want to deal damage to an enemy through a physical attack.
-   As a user, I want to deal damage to an enemy through a magical attack.
-   As a user, I want to deal a reasonable amount of damage to an enemy.
-   As a user, I want to be able to defeat an enemy by reducing its health to 0.
-   As a user, I want to be able to use an item to heal my health or restore magic power.
-   As a user, I shouldn't be able to use a magic attack if my magic power is less than the required amount.
-   As a user, I want to be able to use an item on any ally.
-   As a user, I shouldn't be able to attack an enemy if I'm not close enough.
-   As a user, I shouldn't be able to use an item on an ally if I'm not close enough
-   As a user, I shouldn't be able to move into the area that my allies, enemies or blockades are in.
-   As a user, I shouldn't be able to attack my allies.
-   As a user, I want to be able to run from a battle. 
-   As a user, I want my allies to be able to die so my battle is realistic.
-   As a user, I want to be able to revive my allies.
-   As a user, I want to be able to see my health and MP on a display at the bottom of the screen.
-   As a user, I want to see when my allies' turn is coming next in the turn order bar.
-   As a user, I want to see when my enemies' turn is coming next in the turn order bar.
-   As a user, I want to see information regarding my enemy when the selector is hovering over them.

#### User Animation Stories

-   As a user, I want my physical attacks to have an attacking animation.
-   As a user, I want my magic attacks to have an attacking animation.
-   As a user, I want a using an item animation to play when using an item on an ally.
-   As a user, I want a running animation when moving around the battle.
-   As a user, I want my allies and enemies to have an idle animation in all directions.
-   As a user, I want my attacks or enemies attack to cause the entity to do a stagger animation

## ᛦ State Stack Diagram

[![](https://mermaid.ink/img/pako:eNqdlF1rwyAUhv-KeDnam12GUug-LgYrG3Qw2LKLg54m0kSLmo5S-t9nTFqN3ZYxIRDPed9HOeo5UKY40owaCxbvBBQa6unuOpfEjferDzKdzsmLsBWumEaUq1bXZdOolz5XsI80HhuC5NCFY_gN2Jbj0-ds54tTkTMIUFph9wtrgW2ELMhsxkolGM7n36kf1rdgbKobKk-7SshDUbpsa1hUVR_p9psRsSbggsQ2Wo777yXWlwBso38kvAp5XtUbBRoCGglH4OP2R2VM8LvvZ3u7Uji6px3q6MhPw_NGVWnZWkM4p6E2xAN2ibKJ6iUVqaEQjHyCIaxT_wZJC-EhF4RTwfp7xEqQBZohN93O9_RxzsU9-C8oKbvnuNsdRMfwGz-0ga7XhAfcZ-mE1qhrENz1Dv80c2pLrDGnmfvloDc5zeXR6aCxarWXjGZWNzihzZaHVkOzNVTGRbcg35QKc62aojzPkAur9LJrVb5jHb8AqWJ3AQ?type=png)](https://mermaid.live/edit#pako:eNqdlF1rwyAUhv-KeDnam12GUug-LgYrG3Qw2LKLg54m0kSLmo5S-t9nTFqN3ZYxIRDPed9HOeo5UKY40owaCxbvBBQa6unuOpfEjferDzKdzsmLsBWumEaUq1bXZdOolz5XsI80HhuC5NCFY_gN2Jbj0-ds54tTkTMIUFph9wtrgW2ELMhsxkolGM7n36kf1rdgbKobKk-7SshDUbpsa1hUVR_p9psRsSbggsQ2Wo777yXWlwBso38kvAp5XtUbBRoCGglH4OP2R2VM8LvvZ3u7Uji6px3q6MhPw_NGVWnZWkM4p6E2xAN2ibKJ6iUVqaEQjHyCIaxT_wZJC-EhF4RTwfp7xEqQBZohN93O9_RxzsU9-C8oKbvnuNsdRMfwGz-0ga7XhAfcZ-mE1qhrENz1Dv80c2pLrDGnmfvloDc5zeXR6aCxarWXjGZWNzihzZaHVkOzNVTGRbcg35QKc62aojzPkAur9LJrVb5jHb8AqWJ3AQ)

## Entity State Machine Diagram

[![](https://mermaid.ink/img/pako:eNqFVDtvwjAQ_iuWxwqWjhFCQrQDA0vp1KaDZR-J1dhGzoUKIf57zzHECTVqpnt8990zPnPpFPCCtygQXrSovDDz43NpGX2fT19sPl-yjWpgFwDRPKi9cysqLdeiRW2raC2Y3jPZaPkNipngzsVtEEwGr8mcg791NoP2nc2BSaoq8KMAgShCRLYDd4SVVaseEgHllXZClBnF3-YnI7kV8FODZdh5y6Qz0DJ0TJL7jiOThWIDME6RCUsdQ89DDJpA13aGUWZKHAZ354vefu_TCbBzdCX3unEtvFrXVfW7u4IWC1k7LWG5TOgk3S4nEI-2YEhlLTQg8baKMTqTJ4FyRWRSgEWNJ6ZbZh3SnVAQ2ULU_1RRzJLliVLuB-VPr1XctZSkceZARRN5lCUMK9Np5KYzjHEXPuMGvBFa0d_db7TkWIOBkhckKuG_S17agBMdut3JSl6g72DGu4NKjwEv9qJpyXoQ9sO5pPvQ56CB0uj8Nj4m_Zty-QWMImcN?type=png)](https://mermaid.live/edit#pako:eNqFVDtvwjAQ_iuWxwqWjhFCQrQDA0vp1KaDZR-J1dhGzoUKIf57zzHECTVqpnt8990zPnPpFPCCtygQXrSovDDz43NpGX2fT19sPl-yjWpgFwDRPKi9cysqLdeiRW2raC2Y3jPZaPkNipngzsVtEEwGr8mcg791NoP2nc2BSaoq8KMAgShCRLYDd4SVVaseEgHllXZClBnF3-YnI7kV8FODZdh5y6Qz0DJ0TJL7jiOThWIDME6RCUsdQ89DDJpA13aGUWZKHAZ354vefu_TCbBzdCX3unEtvFrXVfW7u4IWC1k7LWG5TOgk3S4nEI-2YEhlLTQg8baKMTqTJ4FyRWRSgEWNJ6ZbZh3SnVAQ2ULU_1RRzJLliVLuB-VPr1XctZSkceZARRN5lCUMK9Np5KYzjHEXPuMGvBFa0d_db7TkWIOBkhckKuG_S17agBMdut3JSl6g72DGu4NKjwEv9qJpyXoQ9sO5pPvQ56CB0uj8Nj4m_Zty-QWMImcN)

## Class Diagram

[![](https://mermaid.ink/img/pako:eNq1VE2P0zAQ_SuVT4B2V3CtuJRud7WHgkThgnwZOUNi1R5H9gRRSv87dpzWDqVHcknmzfPMm4_4KJRrUCyFMhDCo4bWg5UkaRGfZ7C4IdZ8WLz_fX-_WBlz-LdnQ2gn1wdgNrhjYFxEjxTvHh7eSFEdvsWogiRyckR0ZLzNjF2PxmTGSL5NyaSxqErsMcPp6V3QrF0kSpbcaIsUohnOtkdV3CFp3YLqNGFG1OA9Ej_Fbk1I6L1mDCWDhb4YE39F2kKOe_bosIbAmtoCdQiGu2Kn9FXgkEqs7K99E-W9el2Qz0gN-hpZd0Bt7vkcRrVfO2N0Kv7sOc37l4ZxrOtqtSrmC8U-gtG_cvSpS3WSFTOofY1s3Y8ZY5tCzgoYqDZfGO0NceMeHP-jnL_yVctbZYXYwXr2GFXNAB48ffJxKAUarsbmr8b2EX_yl3i0xi4KPF_DG2puCB9_jEoyjZt72U8XeK72EQ0cqk2JSzqGmIUXd8Kit6CbeIWMwaXgDmNksYyfDfi9FJJOkQcDu92BlFiyH_BO5PKnG0csv4MJEe2BvjlXbO-GtrtY2Gh2fjvdWOl1-gN002kv?type=png)](https://mermaid.live/edit#pako:eNq1VE2P0zAQ_SuVT4B2V3CtuJRud7WHgkThgnwZOUNi1R5H9gRRSv87dpzWDqVHcknmzfPMm4_4KJRrUCyFMhDCo4bWg5UkaRGfZ7C4IdZ8WLz_fX-_WBlz-LdnQ2gn1wdgNrhjYFxEjxTvHh7eSFEdvsWogiRyckR0ZLzNjF2PxmTGSL5NyaSxqErsMcPp6V3QrF0kSpbcaIsUohnOtkdV3CFp3YLqNGFG1OA9Ej_Fbk1I6L1mDCWDhb4YE39F2kKOe_bosIbAmtoCdQiGu2Kn9FXgkEqs7K99E-W9el2Qz0gN-hpZd0Bt7vkcRrVfO2N0Kv7sOc37l4ZxrOtqtSrmC8U-gtG_cvSpS3WSFTOofY1s3Y8ZY5tCzgoYqDZfGO0NceMeHP-jnL_yVctbZYXYwXr2GFXNAB48ffJxKAUarsbmr8b2EX_yl3i0xi4KPF_DG2puCB9_jEoyjZt72U8XeK72EQ0cqk2JSzqGmIUXd8Kit6CbeIWMwaXgDmNksYyfDfi9FJJOkQcDu92BlFiyH_BO5PKnG0csv4MJEe2BvjlXbO-GtrtY2Gh2fjvdWOl1-gN002kv)

## 📐 Wireframes

>[!note]
> Don't go crazy detailed with the wireframes! These should be minimal sketches to convey to the customer what the app will roughly look like. These things tend to change over time as requirements evolve, but you need to start from somewhere.

![picture](ReadmePics/TitleScreen.ong)

Main menu where you can search for a specific rental with a filter button to filter it by size and price. You can scroll down to see more rentals, pressing on the area of the rental brings you to the rental information page. There is a bar at the top to login, see all rentals and to see your rentals, you can also press on the hut logo to go back to the main page (all rentals)

![List View](proposal_photos/IMG_6308.jpeg)

The information page on the rental, it shows the important info of the rental and the price of the rental per night.

![Show View](proposal_photos/IMG_6309.jpeg)

The login view is the initial screen where users can enter their credentials to log into their account. It typically consists of a form with input fields for the username/email and password, along with a "Login" button. The login view should also include a link to the registration page for new users who don't have an account yet.

![Profile View](proposal_photos/IMG_6310.jpeg)

This is the "My Rentals" page that shows your current rentals and previous rentals. You choose between the two by pressing on a button that shows one or the other.

![Profile View](proposal_photos/IMG_6311.jpeg)

This is the checkout page with the location, the start date of your choice if its not taken, then end date of your choice if its not taken and the total price for the amount of nights you're staying.

Javascript controller helper:
https://jsxinput.com/
Sprites:
idk
