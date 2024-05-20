# TWO STEP COMMUNICATION FLOW
Agent Based Modelling for two-step communication flow (Netlogo)

## HOW TO USE?
Download the .nlogo file of the project from [here](https://github.com/aditigarg007/two-step-communication/blob/main/Two%20step%20communication.nlogo). Visit [Netlogo web](http://www.netlogoweb.org/launch) and select the downloaded file after clicking on the _Choose File_ button next to _Upload a model_: option. The screen should look like this -
![Screenshot 2021-09-17 at 2 41 18 PM](https://user-images.githubusercontent.com/39182712/133757219-b7115617-6ebb-43c6-b3b9-a0ee90a5771b.png)

## WHAT IS IT?

The project models the behaviour of two step flow of communication where two media houses A and B influence opinion leaders and opinion leaders influence the general public (opinion followers).

## HOW IT WORKS

1. The two media houses A and B are spread across the patches and are denoted using brown and blue colors respectively. There is no overlap among the patches
2. An adjustable percentage of the population is opinion leaders represented using yellow color, while all other people are represented by white color.
3. Every time an opinion leader comes in contact with a media house, they obtain one message from it.
4. With each tick, opinion leaders can move in any direction upto 10 steps, while opinion followers can move upto 2 steps.
5. The cumulative effectiveness of messages from media house A on an opinion leader is calculated using the product of message-effectiveness-A * messages-A. Similar calculation is done for media house B.
6. For an opnion leader, if cumulative effectiveness of media house A is greater than that of media house B, then they only propagate the messages of media house A. Similarly for media house B.
7. Opinion followers have no direct contact with the media houses and receive messages only from opinion leaders.
8. When opinion followers come in contact with opinion leaders, they obtain messages from all opinion leaders on the same patch.

## HOW TO USE IT

1. Click the SETUP button to setup the agents.
2. Each time the GO ONCE button is pressed, the opinion leaders move upto 10 steps and opinion followers move upto 2 steps increasing the number of ticks by 1.
3. To run go for an infinite amount of time, click GO FOREVER. Click on the same button again to stop the simulation.
4. Population can be varied using the given slider and has a value from 1 to 100.
5. Percentage of the population that acts as opinion leaders can be set using PERCENT-OPINION-LEADERS slider and can vary from 0 to 100.
6. Initial area of influence of media house A can be set up using PERCENT-AREA-A slider. Same holds true for media house B with respect to PERCENT-AREA-B slider.
7. The effectiveness of the messages of the media house can be manipulated by the MESSAGE-EFFECTIVENESS-* slider and can vary from 0 to 1 in steps of 0.1.
8. The monitors depict the number of messages from each media house.
9. The plot depits the number of messages from each media house as a function of time (number of ticks).
 

## THINGS TO NOTICE

Which media house spreads more messages depends on the area of influence of the media house as well as the effectiveness of its messages. Trying out various combinations of the two shows at what point which factor overpowers the other.

## THINGS TO TRY

1. Set up 100% of the population as influencers. This replicates the one step flow model of communication. Since in one step flow communication model, media directly influences people who do not question the medium at all, the effectiveness of the messages of the two media houses is immaterial.
2. Set up 0% of the population as influencers. No messages are propagated.
3. Set up media house population from 0 to 100 and notice the number of messages from each media house.
4. Setting up 0 effectiveness of any media house messages does not give an exponential graph as only influencers are impacted. 

## EXTENDING THE MODEL

One can update the given model to include 

1. Opinion followers being influenced by opinion followers, perhaps not to the extent of influence of opinion leaders.

2. Opinion leaders being impacted by other opinion leaders.

3. Opinion followers directly coming in contact with media houses can also increase awareness.

## RELATED MODELS

Communication-T-T Example


## CREDITS AND REFERENCES

Please cite the NetLogo software as:

Wilensky, U. (1999). NetLogo. http://ccl.northwestern.edu/netlogo/. Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.
