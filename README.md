# **Portfolio**

### About me :wave:
Hi, I'm Anastasiia. 

For the past few years - since 2021 - I've been building my skills and experience in the QA testing. I'm happy that I discovered a field where my love for problem-solving, attention to details, and gaming creates real impact.

There is something special about knowing that your work helps to make user experience with technology/games/applications -smoother and more enjoyable. Through education, independent learning, and hands-on experience, I developed my ability to spot issues and improve digital products throughout different platforms.

This portfolio shows my toolkit and my philosophy: QA isn't just about catching bugs and issues - it's about crafting experiences that people love and raising the quality of the product to ensure that it hits a necessary quality standard before it is delivered to the customer. I'm committed to continuing to work on my growth and leveling up my skills in this field.

[My Linkedin profile](https://www.linkedin.com/in/anastasiia-boiko-kalymon/)

### My experience :office:
My role as a game tester at Gameloft marks my first professional position in QA. 
I have made a significant growth both in my tech and soft skills, such as strong analytical thinking, and developed several testing techniques in AUT testing that were under my responsibility, that resulted in rise of quality of final product and less amount of the Customer Care requests and issues. ✨

I've worked on diverse projects througout diferent stages of SDLC including : Disney Dreamlight Valley (live project), Disney Speedstorm (release stage), and Gangstar New York (development pre-release). As a tester I specialize in game environments, narrative checks, and technical testing(collision, navmesh).

My previous experience, although unrelated to the IT world, has allowed me to develop valuable skills that helped me provide better quality and clearer bug reports that helped with more swift and efficient fixes from the developer's side.

### Tools :wrench:
* [Jira](https://www.atlassian.com/pl/software/jira) - bug tracking
* [Trello](https://trello.com/pl/tour) - project management
* [Confluence](https://www.atlassian.com/software/confluence) - storing information and documents about the project, creating game testing documentations 
* [Mattermost](https://mattermost.com/) - communication within the team
* [Adobe Photoshop](https://www.adobe.com/ca/products/photoshop.html) - complex image attachments creation and editing
* [Google Drive](https://www.google.com/intl/pl_pl/drive/) - storing data
  

### Tech skills :computer:
* [ISTQB Foundation Level](https://sjsi.org/ist-qb/do-pobrania/) knowledge
* Software testing
* Creating test cases
* Reporting bugs
* Creating bug reports
* Performing smoke tests
* Testing AUT
* Regression Testing
  

### Soft skills :file_folder:
* Problem-Solving
* Strong attention to details
* Communication
* Adaptability
* Collaboration
* Empathy


### Certificates :trophy:
* [ISTQB® Certified Tester Foundation Level 4.0 (CTFL)](http://scr.istqb.org/?name=&number=24-CTFL+4-249131-12&orderBy=relevancy&orderDirection=&dateStart=&dateEnd=&expiryStart=&expiryEnd=&certificationBody=&examProvider=&certificationLevel=&country=&resultsPerPage=10)
* [Anti corruption Training](https://drive.google.com/file/d/1EJYuy6ky5z2W1FJ1EBOfbekd0-l058ff/view?usp=sharing)
* [Anti-Harassment and Discrimination Training](https://drive.google.com/file/d/1nVQtJee5huqeL1mIrpdJ5AQqeA7YUVYm/view?usp=sharing)
* [General Data Protection Trainig](https://drive.google.com/file/d/1cnRUl_Ad_gm8y2YlExTIVlNiiIDwutKl/view?usp=sharing)
  
## **Samples of Test Cases :mag:** 
### <ins>**Test Object: Environment**</ins> 

 <ins>**Objective: Make a full technical test coverage of the location and player's interaction with it**</ins>

[Avatar Collision / Navigation mesh]:
- make sure that there is no opportunity to reach inside the textures
- avatar is not clipping with the textures more than is acceptable
- no invisible colliders should be present on location
- there is no unreachable part of navigation mesh where NPC may spawn and become unreachable for player

[Camera collision]:
- make sure that there is no opportunity to reach with camera inside the textures of environment location (floors, walls, ceilings)
- make sure that smaller decorations become invisible upon camera collision to not obscure players view in the center
- there is no invisible colliders present on location (invisible walls)

[Item drop/Grid]:
- items can be dropped in any visually accessible part of the area 
- all items dropped on location can be reachable and can be interacted with 
- fallen items lay on the floor or another designed height and don't show any strange behavior like: disappearing, dropping underground, flying into the air, etc
- fallen items don't clip with the environment or other models

[Natural User behavior]:
- make sure that the avatar can not enter unreachable areas via Tools, Edit Mode, Camera Mode, NPCs, etc
- make sure that the avatar can interact with expected/designed objects of the environment (water-fishing, benches/furniture-sitting animation, walls- climb(if applicable), ground can be dig(if applicable),

[Additional]
- while testing keep an eye on NPC and Mob spawn behavior - if it's present

### <ins>**Test Object: Shop**</ins> 

<ins>**Objective: Unlock/upgrade behavior and players interaction test**</ins>

[Available conditions]:
- the building can be built/restored during the respective requests 

[Unlock]:
- the user can build/restore the building (if applicable)
- the unlock sequence/cutscene is played properly
- currency/resources (if needed) is subtracted correctly

[Upgrade]:
- the buildings have several levels and can be upgraded
- each and every level has its cost and currency/resources are subtracted correctly
- every level has its benefits and are applied correctly, for details consult the Game Development Documentation (further "GDD")

[User behavior and interaction with the building]:
- the building can be entered(if applicable) or interacted with
- correct UI appears and the user can perform the building-related activities, for details consult the GDD

## **Samples of Bug reports :microscope:**

### **Note that all issues mentioned under were found on live build versions of the applications that is available for players without using any cheats or developer builds to respect the NDA contract**

### <ins>**[Unreachable item][NPC House] Items may fall into the unreachable areas in Elsa's Cave**</ins>
* Probability - Common
* Severity - Walkthrough Break
* Reproduction Rate -5/5
* Priority - Blocker

Description :
Items may fall into the unreachable, hard to reach, hard to notice areas in Elsa's House.

Note 1:This issue may become a blocker for players if any of the quest items fall into the unreachable area.

Note 2: This issue is easier to reproduce by dropping the following items: Red Daisy, Garnet.

Steps to Reproduce:
1. * Install and launch the AUT.
2. * Complete FTUE/Tutorial.
3. * Unlock Elsa NPC Character.
4. * Reach Elsa's Cave and enter it.
5. * Open the Inventory and drop items one by one.
6. * Try to pick up all the items.
7. * Notice that items may fall into the unreachable, hard to reach and hard to notice areas in Elsa's House.

For more information please check the attachments below.

Attachments:
![Pic_Items may fall into the unreachable areas in Elsa's Cave](https://github.com/user-attachments/assets/9f7f4b63-2d72-4722-a0c8-0cecd4fc252b)
Note that Video Quality was reduced a lot to fit allowance in 10 Mb.

https://github.com/user-attachments/assets/ab421c7b-c2f4-4ef4-84ec-bc0570e8cb91




### <ins>**[LOC][Premium Shop] "Figaro Bundle" name and description is unlocalized**</ins>
* Probability - Common
* Severity - Medium
* Reproduction Rate -5/5
* Priority - Major

Description :
"Figaro Bundle" and "A unique critter companion to join you on adventures" text strings are missing localization.

Note that this issue occurs with the following languages:
* Francais
* Espanol
* Deutsch
* Italiano
* Japanese
* Chinese
* Portuguese

Steps to Reproduce:
1. * Install and launch the AUT in the affected languages.
2. * Complete FTUE/Tutorial.
3. * Visit the Shop section
4. * Check the 26.03.2025-02.03.2025 Premium Shop items rotation or set specific dates via cheats.
5. * Scroll down the Shop page to reach "Figaro Bundle" items.
6. * Open "Figaro Bundle" to check for more details.
7. * Notice that the "Figaro Bundle" and "A unique critter companion to join you on adventures" text strings are missing localization.

For more information please check the attachments below.

Attachments:
![Pic_Figaro Bundle name and description is unlocalized](https://github.com/user-attachments/assets/7ddd1209-3ee0-4f9d-98a6-53a49842333e)

https://github.com/user-attachments/assets/8e1d3504-0fa2-462d-89e6-59e4b0e56b02




### <ins>**[Navmesh][Mulan Realm] Gap in navigation mesh is present in the Mulan Realm**</ins>
* Probability - Common
* Severity - Medium
* Reproduction Rate -5/5
* Priority - Major

Description :
There is an opportunity to reach behind the textures through the gap without collision in the Mulan Realm.

Steps to Reproduce:
1. * Install and launch the AUT.
2. * Complete FTUE/Tutorial.
3. * Unlock Mulan Realm and enter it.
4. * Reach to location mentioned in the attachments.
5. * Attempt to pass through the area.
6. * Highlight the Item.
7. * Take a closer look at the highlight shape.
8. * Notice that there is an opportunity to reach inside the textures on the Mulan Realm.

For more information please check the attachments below.

Attachments:
![Pic_Gap in navigation mesh is present in the Mulan Realm](https://github.com/user-attachments/assets/00bc76b5-4f03-44a4-9ff1-e159932209c8)


https://github.com/user-attachments/assets/42c124e7-f5c1-47f6-a9f6-7e543a46a78b




### <ins>**[Furniture][Edit Mode] Vitalys Mines Lamp has corrupted highlights in Edit Mode**</ins>
* Probability - Common
* Severity - Medium
* Reproduction Rate -5/5
* Priority - Major

Description :
The highlight of Vitalys Mines Lamp does not match its model and has square highlights for VFX in Edit Mode.

Note 1:This issue may become a blocker for players if any of the quest items fall into the unreachable area.

Note 2: This issue is easier to reproduce by dropping the following items: Red Daisy, Garnet.

Steps to Reproduce:
1. * Install and launch the AUT.
2. * Complete FTUE/Tutorial.
3. * Obtain the Vitalys Mines Lamp by buying it in the Scrooge Store.
4. * Place the Vitalys Mines Lamp on the grid in Edit Mode.
5. * Open the Inventory and drop items one by one.
6. * Highlight the Item.
7. * Take a closer look at the highlight shape.
8. * Notice that the Vitalys Mines Lamp has corrupted highlights in Edit Mode.

For more information please check the attachments below.

Attachments:
![Pic_Vitalys Mines Lamp has corrupted highlights in Edit Mode](https://github.com/user-attachments/assets/45b07c4e-dc75-477d-80fa-0e1705ba591f)

https://github.com/user-attachments/assets/8b0d0970-df22-4325-940e-fa00ba61bc69




### <ins>**[NPC Houses][Monster Incorporation]Camera has no collision with the staircase of the Mike's at Sulley's House**</ins>
* Probability - Common
* Severity - Minor
* Reproduction Rate -5/5
* Priority - Minor

Description :
The camera has no collision with the staircase/stone balustrades of Mike's at Sulley's House.

Steps to Reproduce:
1. * Install and launch the AUT.
2. * Complete FTUE/Tutorial.
3. * Reach Step 15 of the "Eye on the Prize" Monster Incorporation Realm Request and place the Mike's and Sulley's *House in the Valley.
4. * Reach Mike and Sulley's House.
5. * Move the camera into the staircase of the House, as shown in the attachment.
6. * Notice that camera has no collision with the staircase/stone balustrades of the Mike's at Sulley's House.

For more information please check the attachments below.

Attachments:

![Pic_The camera has no collision with the staircasestone balustrades of Mike's at Sulley's House](https://github.com/user-attachments/assets/437d7bc8-6e31-435f-8345-1fb6ba1a3aef)

https://github.com/user-attachments/assets/ce054475-0a17-4c51-9be1-7aa8c437a293


### Thank you for your attention!
