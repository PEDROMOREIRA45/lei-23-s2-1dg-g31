# US 007 - Register in the system 

## 1. Requirements Engineering


### 1.1. User Story Description


As an unregistered user, I want to register in the system to buy, sell or rent
properties.


### 1.2. Customer Specifications and Clarifications 


**From the specifications document:**

>	All those who wish to use the application must be authenticated with a password of seven alphanumeric characters, including three capital letters and two digits.




**From the client clarifications:**

> **Question:** In the project's documentation it's mentioned that "All those who wish to use the application must be authenticated", but in the US1 it's said that an unregistered user can see a list of properties. Can users who aren't authenticated do this?
>  
> **Answer:** Non-authenticated users can only list properties.


### 1.3. Acceptance Criteria


* **AC1:** Unregistered user must have an unique email.
* **AC2:** Unregistered user must obey password rules.

### 1.4. Found out Dependencies


* None


### 1.5 Input and Output Data


**Input Data:**

* Typed data:
	* Email
    * Password
	
* Selected data:
    * Choosing business type (sell or lease)
    * Choosing type of property
    * Choosing number of bedrooms
    * Choosing sort type


**Output Data:**

* List of listed properties

### 1.6. System Sequence Diagram (SSD)

![System Sequence Diagram](./svg/us001-system-sequence-diagram-System_Sequence_Diagram__SSD.svg)

### 1.7 Other Relevant Remarks

* Unregistered users can only see the listed properties. They can't bid on properties unless they authenticate. 