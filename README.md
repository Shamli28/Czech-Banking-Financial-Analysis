# Czech-Banking-Financial-Analysis

Data Analysis of Real Czech Bank

## Introduction
For Banks, it is always an interesting & challenging problem to predict how likely a client is going to default the loan when they only have a handful of information.

## Motivation
Customer Age and Gender Population overview.
We can identify most attractive districts in Czech for future.
Probability of a loan turning into default.
Credit department efficiency overview within country: which districts are giving mostly “good” or “bad” loans.
Bank’s funds inflows and outflows analysis. Does the bank face negative cash flow rarely or often? Is there any patterns for funds outlaying?

## Install

This project requires Python 3.x and the following Python libraries installed:

 1. NumPy
 2. Pandas
 3. Matplotlib
 4. Seborn
 5. Plotly
 6. Collections
    
## Data

Data from a real Czech bank. From 1999. Reported period 1993 - 1998. The data about the clients and their accounts consist of following relations:

 - relation account (4500 objects in the file ACCOUNT.CSV) - each record describes static characteristics of an account, 
 - relation client (5369 objects in the file CLIENT.CSV) - each record describes characteristics of a client,  
 - relation disposition (5369 objects in the file DISP.CSV) - each record relates together a client with an account i.e. this relation describes the rights of        clients to operate accounts,
 - relation permanent order (6471 objects in the file ORDER.CSV) - each record describes characteristics of a payment order,
 - relation transaction (1056320 objects in the file TRANS.CSV) - each record describes one transaction on an account,
 - relation loan (682 objects in the file LOAN.CSV) - each record describes a loan granted for a given account,
 - relation credit card (892 objects in the file CARD.CSV) - each record describes a credit card issued to an account,
 - relation demographic data (77 objects in the file DISTRICT.CSV) - each record describes demographic characteristics of a district. Each account has both static    characteristics (e.g. date of creation, address of the branch) given in relation "account" and dynamic characteristics (e.g. payments debited or credited,        balances) given in relations "permanent order" and "transaction". Relation "client" describes characteristics of persons who can manipulate with the accounts.    One client can have more accounts, more clients can manipulate with single account; clients and accounts are related together in relation "disposition".          Relations "loan" and "credit card" describe some services which the bank offers to its clients; more credit cards can be issued to an account, at most one loan    can be granted for an account. Relation "demographic data" gives some publicly available information about the districts (e.g. the unemployment rate);            additional information about the clients can be deduced from this.

## Data dictionary

List of datasets and data dicitonary can be found in Data dictionary.pdf


