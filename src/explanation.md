# Hospital Management System

This project is a Hospital Management System built using Spring Boot. It provides a set of RESTful APIs to manage various aspects of a hospital, such as addresses, branches, encounters, hospitals, medical items, medical orders, and persons.

## Features and Functionality

### Addresses
- **Save**: Add a new address.
  - `POST /address`
- **Update**: Modify an existing address using its ID.
  - `PUT /address?id={id}`
- **Delete**: Remove an address using its ID.
  - `DELETE /address?id={id}`
- **Get**: Retrieve an address using its ID.
  - `GET /address?id={id}`

### Branches
- **Save**: Add a new branch linked to a specific hospital and address.
  - `POST /branch/{hid}/{aid}`
- **Update**: Modify an existing branch using its ID.
  - `PUT /branch?id={id}`
- **Delete**: Remove a branch using its ID.
  - `DELETE /branch?id={id}`
- **Get**: Retrieve a branch using its ID or get all branches linked to a specific hospital ID.
  - `GET /branch?id={id}`
  - `GET /branch/{hid}`

### Encounters
- **Save**: Add a new encounter (interaction between a patient and the hospital) linked to a specific person and branch.
  - `POST /encounter?pid={pid}&bid={bid}`
- **Update**: Modify an existing encounter using its ID and branch ID.
  - `PUT /encounter?id={id}&bid={bid}`
- **Delete**: Remove an encounter using its ID.
  - `DELETE /encounter?id={id}`
- **Get**: Retrieve an encounter using its ID.
  - `GET /encounter?id={id}`

### Hospitals
- **Save**: Add a new hospital.
  - `POST /hospital`
- **Update**: Modify an existing hospital using its ID.
  - `PUT /hospital?id={id}`
- **Delete**: Remove a hospital using its ID.
  - `DELETE /hospital?id={id}`
- **Get**: Retrieve a hospital using its ID.
  - `GET /hospital?id={id}`

### Medical Items (MedItems)
- **Save**: Add new medical items linked to a specific medical order.
  - `POST /meditems?mid={mid}`
- **Update**: Modify existing medical items using their ID.
  - `PUT /meditems?id={id}`
- **Delete**: Remove medical items using their ID.
  - `DELETE /meditems?id={id}`
- **Get**: Retrieve medical items using their ID.
  - `GET /meditems?id={id}`

### Medical Orders (MedOrder)
- **Save**: Add a new medical order linked to a specific encounter.
  - `POST /medorder?eid={eid}`
- **Update**: Modify an existing medical order using its ID.
  - `PUT /medorder?id={id}`
- **Delete**: Remove a medical order using its ID.
  - `DELETE /medorder?id={id}`
- **Get**: Retrieve a medical order using its ID.
  - `GET /medorder?id={id}`

### Persons
- **Save**: Add a new person (patient or staff).
  - `POST /person`
- **Update**: Modify an existing person using their ID.
  - `PUT /person?id={id}`
- **Delete**: Remove a person using their ID.
  - `DELETE /person?id={id}`
- **Get**: Retrieve a person using their ID.
  - `GET /person?id={id}`

## How to Use the Project
1. **Setup**: Clone the repository, build the project using Maven, and run the application.
2. **Access the APIs**: Use tools like Postman or a web browser to interact with the various endpoints listed above.
3. **Swagger Documentation**: Access `http://localhost:8080/swagger-ui.html` to see interactive API documentation, which makes it easy to test and understand the endpoints.

## Example Usage
- To save a new hospital, you would send a `POST` request to `/hospital` with the hospital details.
- To update an existing branch, you would send a `PUT` request to `/branch?id={id}` with the branch's new details.
- To get details of a specific encounter, you would send a `GET` request to `/encounter?id={id}`.

This project helps manage and organize the hospital's data efficiently, allowing for easy addition, modification, retrieval, and deletion of records through a set of well-defined APIs.

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.
