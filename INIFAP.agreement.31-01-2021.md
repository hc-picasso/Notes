---
id: NIrrVVxaOAH0yF1c65yNi
title: 31-01-2021
desc: ''
updated: 1643905117329
created: 1643652799500
---

Ramón sent answer back from questions along with the new technical proposal.

Q: Do you think we can use a power of attorney as the legal designation?

A: Only if it is explicit in the document.

Q: We have a one pager of HC's purpose mission and vision, would that be useful for purpose statement?}

A: Yes, please give me the address.

Q: As following is how HC envisions publications:
Please let us know your thoughts on the proposed publication timelines and conditions for the 1st and 2nd publications. My understanding last meeting was that it would be better to keep the data for some time before publishing it for the best outcome of Publication 3 and/or 6 -Please correct me if I'm wrong-. I think it would be good for us to talk more about this in a forthcoming meeting. 

A: Please, include state this into the body of the agreement. Once the department of legislation of INIFAP check it, you will know if it is possible or not. As a technical part, I can see this is feasible, but let see if they also think it is possible.

Q: Regarding the seventh clause, we'd like to ask more specifically how would IP right-holding be at the end of the day for the publications (i.e. patrimonial rights) and the other forms of IP mentioned therein.

A: It is very similar to the previous question, because it is a project paid by you and implemented by us. Together, we can propose how the results of this project will be used, what is your proposal? Please include it in this section, and based on that proposal, let's build a joint proposal.

Q: Regarding the payments, if a Mexican entity were to provide such payments, would there be an increase because of taxes? or would it be the same amount of money?

A: There are two types of projects to be carried out by INIFAP, Research and Service. This is a Research project and there will be no TAX cost, I have just been informed. It does not matter if it is a Mexican or Foreign entity.


## Daniel Notes

- What is CE Altos de Jalisco & Valle de Mexico?
- Who is going to keep the equipment.
- If research has no taxes, should we remove the IVA part of the final quote?
- where chronogram?
- Initial determination (15 plants) would be 135 samples cogollo, 540 samples unfolded penca, 45 samples piña [$67,806 MXN]
    - Proposing alternative Lab?
    - Figures don't add up: $44,500.00 + $25,056.00 = 69,566 <> Total: $ 67,806.00 | What's with this: Subtotal: $12,500.00?
- Destructive sampling of 120 plants (120 sample piña and 360 sample penca) [Total: $9000.00 + $213,006.00 Where is that cmming from? What is the green text?]
    - Still proposing the cheaper method for carbon
    - Output: allometric models, R, R2, RCME
    - CE Jalisco y México?
    - LECO method is NOT the one quoted
    - We can use EMLID GNSS to get correct geoppositioning instead of GPS Garmin
- Inventory [Subtotal: $ 94,500.00 | 2000+35000+8000+2400+5000+44100=96500]
- Drone Flights : $251,400
- Error propagation: $120,000
- What CRS do you recommend?

# Michael Notes

Notes:

Overall note: you and I need to meet to discuss all the budget items listed here

Figure 1, is this the correct field boundary?

- I think we should remove every time “mezquite” is mentioned, there are no mezquite at don Rubens
- (Flores et al., 1995; Rojas-García et al., 2015; Valles et al., 2011) are these the alometric equations we plan to use? Or are they just general references?
- 3 groups of plants: I think it’s more relevant to group them by size (ie height). I don’t think we should exclude the smallest plants, I think they should just be part of the smallest group

Humidity sampling:
- will these samples be tested for carbon? It’s important to me that they are, if so what method of carbon analysis?
- I don’t understand how the 3 pencas will be taken from the cogollo. One from the outtermost, one in the middle, and 1 innermost?
- I think we need more samples per pina, 3 cubes from each section (top middle and bottom), total of 9 samples per pina.
- is 75 degrees C the standard practice? If so that’s fine.
- why do we have the option between CENID-RASPA and CEBAJ for the same analysis?
- I’m confused by the Valle de Mexico travel expenses

Estimation of volume/biomass/carbon:

- volume measurements are never mentioned
- in the first section roots are mentioned, but they will be excluded from this study
- let’s make sure all the variables we want are included in “variables físicas de fácil acceso”
- 120 plants sounds good, but will they be equally distributed across ages, or more weighted to older larger plants? Weighting to larger plants works for me
- 3 samples per pencas sound a little excessive to me, but that’s fine (depending on total cost)
- depending on the cost, we can exclude azucares totales
- we DONT want to test for OM, we want to test using dumas dry combustion 
- I don’t understand the plan for using the random forest model (do you Daniel) 
- I don’t understand altos de Jalisco or Valle de Mexico budget sections
- can we do this work in the same chunk of time as the inventory and drone flights? If so, what’s the total timeframe of that chunk of work?

Inventory:

I’m a little unclear how this will actually work.
Here is my understanding

- 200 plots will be selected (what size are these plots?)
- Number of agave (huizache & nopal) will be counted in each plot
- diameter x2 and height will be measured for each agave (what will be measured for huizache and nopal?)
- Agave density will be extrapolated to the entire field area, and specific agave data will be used to compare to the drone imagery (to correct for height, diameter, and detection) 

For huizache & nopal:
- 5 individuals sampled sounds good, what size will these individuals be? Will they be weighted towards the larger size plants? That’s fine with me.
- How will we calculate dry biomass (based off the methods of the alometric equations we are referencing)
- will we measure C on these samples?
- how will we create the alometric equation to drone characterization model? (I.e. dbh to crown canopy) We will measure 30 individuals? Of different size ranges? 30 individuals works for me, so long as the 3 alometric equations we are referencing use the same variables (I.e. dbh)
- Garmin gps seems obsolete

Drone:
-RGB 4cm 
-sequoia 6cm 
-I thought it was 3cm and 5cm, but okay…
-drone flights before and after inventory sampling, does this double our cost? Is this really necessary?
-cost of the drone flights is unfortunately high in my opinion. Does this include training to Hc to use the code inifap creates? How much image processing is included in this cost? Does this include a C estimation of huizache and nopal? 
-it seems like inifap will not be processing any of our phantom 4 drone data?

Error estimation:
-is it possible that Daniel and Mike help with the sampling? If we are trained with the proper methodologies? 
-Can we be more specific about the expected sources of error in each section 
(In example:
Drone errors- imaged vs measured agave height and diameter, error in drone gps accuracy (1-2cm))
-can we provide more detail how the método GUM and the Monte Carlo simulations will be used?