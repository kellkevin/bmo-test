** Scenarios **

2.   Feature: Use the website to find restaurants
3.            So that I can order food
4.            As a hungry customer
5.             I want to be able to find restaurants in my area

6.  	Scenario: Search for restaurants in an area
7.            Given I want food in "AR51 1AA"
8.            When I search for restaurants
9.            Then I should see some restaurants in "AR51 1AA"

Scenario: See the menu details for a restaurant
	Given I want food in "AR51 1AA"
	When I search for restaurants
	And Click on a restaurant result
	Then I should see the menu of the restaurant 

Scenario: Invalid Address
	Given I want food in an invalid address
	When I search for for restaurants with a fake address
	Then I should see an error.


** How long did you spend on the technical test? **
About over an hour. 

** What would you add to your solution if you had more time? If you didn't spend much time on the technical test then use this as an opportunity to explain what you would add. **
- I would probably aim for a more end-to-end test where it covers login scenarios and the full order. EVen the registration and actual ordering to test out the system. Even more error scenarios.

** What do you think is the most interesting trend in test automation? **
Codeless testing. Which is pretty much the solution that I ended up using. Less time attempting to understand the overbearing ins-and-outs of the subject to use. Seeing the apps do recording. 

** How would you implement test automation in a legacy application? Have you ever had to do this? **
I would gather high level scenarios and starting with those. 

How would you improve the customer experience of the JUST EAT website?
- enabling the ability to search the FAQs without having a login. 
- reseting the form would not need a reloading of the page 
- grabbing the data in an ajax call for the search instead of postbacks.
- less demos 

** Please describe yourself using JSON. **

{
	"name": "kevin",
	"age": "NaN",
	"occupationData": {
		"role": "front end developer"
		"skills": ["html","jquery","php","css3"]
	},
	"country": "Canada",
	"residence": "Etobicoke",
	"favoriteFoods": ["mexican","thai"],
	"bestAttribute": ["telling jokes", "doing tricks"],
	"quote": "no fellow candle sticks",
	"other":""
}


