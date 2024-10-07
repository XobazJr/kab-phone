# Project KAB Phone

The project is a mobile phone e-commerce website developed as an assignment for the SA course. The instructor is Asst. Prof. Khantharat Anekboon, Ph.D.


## Requirement 

| Stakeholder | Hardware | Input | Output | Functional requirement | Nonfunctional requirement | When |
| :-------- | :-------- | :-------- |:-------- | :--------|:-------- | :--------|
| Admin |           | New phone data |           | An admin adds new phone to stock or remove outdated phone from stock |           | They launched a new phone or there is an outdated phone |
| Admin |           | Tracking number |           |           |           | Paid order occurred |
| Customer | Payment,Address,Tel no. |           |      Updated stock,Invoice receipt |           | When customer add item to basket. It will not deduct from stock until payment success | Daily |
| Customer | Name,Address,Tel no.,Line ID |           |           |           | Customer can edit name, address, Tel no., or Line ID | Daily |

## 1 Usecase

<img hight="297" width="210" src="https://github.com/xobazjr/kab-phone/blob/main/assets/use-case.jpg">

## 2 Fully usecase description

| Use Case Name: | Add item to basket |                                                                                                                                        |
| :-------- | :-------- | :--------                                                                                                                                            |
| Scenario: | Customer adding item to basket and see the total price. |                                                                                                        |
| Triggering Event: | Customer adds an item into the basket. |                                                                                                                 |
| Brief Description: | First, customer click add an item into the basket. Then the system will return item price and item description. Then calculate total price. |           |
| Actors: | Customer |                                                                                                                                                         |
| Related Use Cases: | Including: Stock Check, Item Description |                                                                                                              | 
| Stakeholders: | Admin: to provide description related to that item from stock. |                                                                                             |
| Preconditions: | Item that customer added. |                                                                                                                                 |
| Postconditions: | -	Show an error if item is out of stock. |                                                                                                                 |
| Flow of Activities: | Actor | System                                                                                                                                         |
|           | 1.	Customer is looking for a wanted item from the store front page. |                                                                                           |
|           | 2.	Customer clicked add item to the basket. 2a. if out of stock, go back to step 1. | 2.1 System check if item is not empty.                                    |
|           | 2.2 Then return the price to customer. | 2.2	Then return the price to customer.                                                                                 |
|           | 3.	Customer adds quantity they want into the specified item in the basket. |                                                                                    | 
|           | 4.	Customer place an order. |                                                                                                                                   |
| Exception Conditions: | 2. When item is out of stock. |                                                                                                                      |
|           | 3. When item is not enough in stock. |                                                                                                                           |

##
<br/>

| Use Case Name: | Place Order |                                                                                                                                                               |
| :-------- | :-------- | :--------                                                                                                                                                            |
| Scenario: | Customer is adding item into basket, then make a payment. |                                                                                                                      |
| Triggering Event: | Add an item into the basket |                                                                                                                                            |
| Brief Description: | At first, customer is select the prefer item. Then add it into basket. System will check if item is ready for sell. If yes user will make payment, and done |           |
| Actors: | Customer |                                                                                                                                                                         |
| Related Use Cases: | Including: Stock Check, Item Description, Payment |                                                                                                                     | 
| Stakeholders: | Admin: to provide stock, and item description. |                                                                                                                             |
|  | Bank: to provide payment process. |                                                                                                                                                       |
| Preconditions: | Item that customer added. |                                                                                                                                                 |
| Postconditions: | -	Show an error if item is out of stock.          |                                                                                                                        |
|  | -	Show an error if payment process failed.          |                                                                                                                                    |
|  | -	Show success page if everything goes correctly.          |                                                                                                                             |
| Flow of Activities: | Actor | System                                                                                                                                                         |
|           | 1.	Customer selects an item. |                                                                                                                                                  |
|           | 2.	Customer add it into basket. | 2.1 System check for stock.                                                                                                                   | 
|           | 3.	Customer confirm an order. | 2.2 If stock is empty then return to customer.                                                                                                  | 
|           | 4.	Customer making a payment. 4a. if payment failed, goes to 2. | 4.1 System contact the payment provider.                                                                      |
|           | 5.	Order placement success. | 4.2 System return payment status.                                                                                                                 |
| Exception Conditions: | 2. When item is out of stock. |                                                                                                                                      |
|           | 4. When payment is not success. |                                                                                                                                                |


## Context diagram 

<img hight="500" width="500" src="https://github.com/xobazjr/kab-phone/blob/main/assets/context-diagram.jpg">

## DID Level 0

<img hight="500" width="500" src="https://github.com/xobazjr/kab-phone/blob/main/assets/dfd-level-0.jpg">

## 2 Sequence diagrams are based on 2 Use case descriptions

<img hight="500" width="500" src="https://github.com/xobazjr/kab-phone/blob/main/assets/sequence-diagram-ssd-0.1.jpg">

<img hight="500" width="500" src="https://github.com/xobazjr/kab-phone/blob/main/assets/sequence-diagram-ssd-0.2.jpg">

## Interface

<img src="https://github.com/XobazJr/kab-phone/blob/main/interface/png/user-interface.png">

## Testing

<img hight="500" width="500" src="https://github.com/xobazjr/kab-phone/blob/main/assets/interface-structure-diagram.jpg">



