# HealthMatrix

## Project Overview

This project is a Hospital Management System developed using Spring Boot. It consists of several RESTful APIs to manage hospital-related data, including addresses, branches, encounters, hospitals, medical items, medical orders, and persons. The project uses Spring Data JPA for data persistence and Swagger for API documentation.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Usage](#usage)


## Features

- CRUD operations for Address, Branch, Encounter, Hospital, MedItems, MedOrder, and Person entities.
- API endpoints secured with validation annotations.
- API documentation with Swagger.
- RESTful API design.
- Modular service-oriented architecture.

## Technologies Used

- Java 
- Spring Boot 
- Spring Data JPA
- Hibernate
- Maven
- Postman


## usage

### Save Address

`POST /address`

### Update Address

`PUT /address?id={id}`

### Delete Address

`DELETE /address?id={id}`

### Get Address By Id

`GET /address?id={id}`

## Branch Endpoints

### Save Branch

`POST /branch/{hid}/{aid}`

### Update Branch

`PUT /branch?id={id}`

### Delete Branch

`DELETE /branch?id={id}`

### Get Branch By Id

`GET /branch?id={id}`

### Get Branch By Hospital Id

`GET /branch/{hid}`

## Encounter Endpoints

### Save Encounter

`POST /encounter?pid={pid}&bid={bid}`

### Update Encounter

`PUT /encounter?id={id}&bid={bid}`

### Delete Encounter

`DELETE /encounter?id={id}`

### Get Encounter By Id

`GET /encounter?id={id}`

## Hospital Endpoints

### Save Hospital

`POST /hospital`

### Update Hospital

`PUT /hospital?id={id}`

### Delete Hospital

`DELETE /hospital?id={id}`

### Get Hospital By Id

`GET /hospital?id={id}`

## MedItems Endpoints

### Save MedItems

`POST /meditems?mid={mid}`

### Update MedItems

`PUT /meditems?id={id}`

### Delete MedItems

`DELETE /meditems?id={id}`

### Get MedItems By Id

`GET /meditems?id={id}`

## MedOrder Endpoints

### Save MedOrder

`POST /medorder?eid={eid}`

### Update MedOrder

`PUT /medorder?id={id}`

### Delete MedOrder

`DELETE /medorder?id={id}`

### Get MedOrder By Id

`GET /medorder?id={id}`

## Person Endpoints

### Save Person

`POST /person`

### Update Person

`PUT /person?id={id}`

### Delete Person

`DELETE /person?id={id}`

### Get Person By Id

`GET /person?id={id}`


