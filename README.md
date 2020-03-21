# ROZGAAR-APP 

## Abstract
In India, the daily wage labourers are large in number and their entire day-to-day activities are dependent on the wages they get from daily works. The problem is that due to the large number of workers and them being in small towns many labourers can not get work. So our idea is to not let the labourers search the work but the work to search the labourers.
We have design an application in which contractors will ask for labourers with required skills and based on that we’ll inform the appropriate labourers about the work and its details like, estimated pay, location, type of work etc. Thus any work from nearby areas can be made accessible to the labourers easily.

## Solution Approch 
One of the solutions to the above problem is to make a database of the labourers location wise including details such as their skill, age, gender, working capability, income, phone-number, address etc.

On the contractor's side, a flutter based mobile app will be there which will take the details from the contractor such as work type, address of work, number of labourers, amount (satisfying the minimum wage act ) etc. These details will be sent to the flask server where first the nearest places to the contractor’s address will be sorted using the map API.

After sorting the places, the labourers will be chosen based on their skill which is required for the specific work. The selected labourers will be then selected by the machine learning modelSorted laborers according to location are fed into the ML model. The model will be trained on parameters like age, capability, their income till now, etc  the selected laborers will either receive notification in the app, message in phones, calls using the respective APIs. The labourers can accept or reject the offer and the required number of labourers would be selected using ‘first come first serve’ basis. The model will be trained in a way that all the labourers get equal opportunities.

After the work is done, feedback from the contractor will be taken and the database of the labourer will be modified accordingly. On the labourer’s side, they will have the option to complain against exploitation or any other issue.
Along with labours, it would be a convenient method for contractors as well and will help in suggesting relevant and nearby labourers according to job requirements and location  which will ultimately increase their productivity.

## Block Diagram
![200x150](https://github.com/silentkiller101099/open-innovation-rozgaar/blob/master/img/Block%20diagram.jpg "Block Diagram")

## Tech Stack 
- Flask
- Flutter
- SQLite3
- Google Map API
- Sklearn

## Future Goals
- Ensuring correct information on each labourer’s and contractor’s side.
- Automatic skill selection using only work type.
- Not only in labour, but also in other fields increasing employment.


## Repositories Files
There are 3 folders and a main.py for running test.

- database (Includes the database files)
- model (Include the ML model files which will predict the scores of laborers)
- rozgaar (Includes all flutter files for the app design)

         
