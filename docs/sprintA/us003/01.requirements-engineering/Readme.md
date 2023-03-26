# US 003 - Register a new employee

## 1. Requirements Engineering


### 1.1. User Story Description


As a system administrator, I want to register a new employee


### 1.2. Customer Specifications and Clarifications 


**From the specifications document:**

>	The company's systems administrator will be responsible for registering all employees (specifying the name, the citizen's card number, the tax number, the address, the email address, the contact telephone number and the agency to which it is assigned).


**From the client clarifications:**

>	**Question:** The administrator when registering a new employee will also have to specify the category/office that he will perfom (for example agent, store manager, store network manager)?
>  
>	**Answer:** The administrator has to specify the role of the employee.


### 1.3. Acceptance Criteria


* **AC1:** All required fields must be filled in.
* **AC2:** All data must be valid.


### 1.4. Found out Dependencies

* There are no dependencies.

### 1.5 Input and Output Data


**Input Data:**

* Typed data:
	* a name, 
	* a citizen card number, 
	* a tax number,
	* an address,
	* an email address,
	* a telephone number,
    * an agency


* Selected data:
	* The user's role


**Output Data:**

* (In)Success of the operation

### 1.6. System Sequence Diagram (SSD)

**Other alternatives might exist.**

#### Alternative One

![System Sequence Diagram - Alternative One](svg/us003-system-sequence-diagram-alternative-one.svg)

#### Alternative Two

![System Sequence Diagram - Alternative Two](svg/us003-system-sequence-diagram-alternative-two.svg)

### 1.7 Other Relevant Remarks

* The created task stays in a "not published" state in order to distinguish from "published" tasks.