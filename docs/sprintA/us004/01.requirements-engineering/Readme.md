# US 006 - Owner submit a request for listing a property  

## 1. Requirements Engineering


### 1.1. User Story Description


As an owner, I intend to submit a request for listing a property sale or rent,
choosing the responsible agent.

### 1.2. Customer Specifications and Clarifications 


**From the specifications document:**

From time to time, property owners contact Real Estate USA with the aim of selling or renting their properties. Owners go to one of the company's branches and meet with a real estate agent to sell or rent one or more properties, or they can use the company's application for the same purposes.
The owner provides property characteristics and the requested price and sends the request to an agent. 
In the case of a request for the sale of a property, the owner must provide information on: the type of property (apartment, house or land), the area in m2, the location, the distance from the city centre, the requested price and one or more photographs.
If the property is an apartment or a house, the owner also provides: the number of bedrooms, the number of bathrooms, the number of parking spaces and the available equipment, such as central heating and/or air conditioning. 
In case the property is a house, the existence of a basement, an inhabitable loft, and sun exposure must be registered as well.

**From the client clarifications:**

> **Question:** Are there any restrictions on the choice of an Agent?
>  
> **Answer:** No.

> **Question:** In case the submission of the listing is online may the owner choose any agent?
>  
> **Answer:** Yes.

> **Question:** In case it is on an agency, must the agent be assigned automatically by the system?
>
> **Answer:** The agent that registers the information in the system can choose to assign any agent.

> **Question:** We are having a little issue defining what the sun exposure might be. We are not sure what it will be as a value. If it's a number that defines how much exposure the house has or if it is just a text saying if it has or hasn't sun exposure.
>
> **Answer:** Sun exposure will take the following values: North, South, East, or West.
 

### 1.3. Acceptance Criteria


* **AC1:** The Owner has to chose a Store.
* **AC2:** The Owner has to chose a Agent from a list of Agents in that Store.
* **AC3:** The store is registered branch by the Systems Administrator.
* **AC4:** An Agent is registered employee by the Systems Administrator.
* **AC5:** An Agent is a employee of that store.
* **AC6:** The Owner has to provide all de required information.
* **AC7:** In the case of a request for the sale of a property, the owner must provide information on: the type of property (apartment, house or land), the area in m2, the location, the distance from the city centre, the requested price and one or more photographs.
* **AC8:** If the property is an apartment or a house, the owner also provides: the number of bedrooms, the number of bathrooms, the number of parking spaces and the available equipment, such as central heating and/or air conditioning.
* **AC9:** In case the property is a house, the existence of a basement, an inhabitable loft, and sun exposure must be registered as well.
* **AC10:** All required fiels must be filled in.


### 1.4. Found out Dependencies


* There is a dependency to " US3: As a system administrator, I want to register a new employee. " since the Agent has to be a registered employee by the Systems Administrator.
* There is a dependency to " US5: As a system administrator, I want to register a store.  " since the Store has to be a registered branch by the Systems Administrator.
* There is a dependency to " US6: As a system administrator, I want to specify districts, municipalities, and parishes in the system." since the information of the property needs identification of districts, municipalities, and parishes.

### 1.5 Input and Output Data


**Input Data:**

* Typed data:
	* reference, identification property.
    * number of bedrooms.
    * number of bathrooms.
    * number of parking spaces.
    * area (mts2).
    * distance from the city centre (kilometres).
    * prequested price (currency).
    * photos(images).

	
* Selected data:
	* propertytype chose: 1 – apartment; 2 – house; 3 – land. 
    * propertyTypeInSunExposure chose: 1 – North, 2 – South, 3 – East, 4 – West.
    * propertyTypeInhabitable: yes or no inhabitable loft. 
    * propertytypecentralheat: yes or no central heating.
    * propertytypeaircond: yes or no air conditioning.
    * propertytypebasement: yes or no basement.
    * idlocation: identifies location.
    * idcodagent: identification agent.


**Output Data:**

* Document with Confirmation of registration of the property 

### 1.6. System Sequence Diagram (SSD)

**Other alternatives might exist.**

#### Alternative One

![System Sequence Diagram - Alternative Two](svg\us004-system-sequence-diagram-alternative-one-System_Sequence_Diagram__SSD____Alternative_One.svg)

#### Alternative Two

![System Sequence Diagram - Alternative Two](svg\us004-system-sequence-diagram-alternative-two-System_Sequence_Diagram__SSD____Alternative_Two.svg)

### 1.7 Other Relevant Remarks

* This task can be performed by the Owner directly in the application (needs to identify store and agent), or can be performed with a agent in the store.