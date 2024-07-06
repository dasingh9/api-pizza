# Pizza Orders API

This is a simple REST API for managing pizza orders using Node.js and Express.
We can get, create, update, and delete pizza orders using this REST API.

## General Instructions

You will need to think about:
- USE MVC folder structure for your API project
  - Here's a sample API for your reference: ```https://github.com/dasingh9/games-api```
- Use dummy data for testing your APIs.
- Test in Postman to make sure all is working correctly.
- Don’t forget to use `.gitignore`, so that the `node_modules` folder is not uploaded to your remote GitHub repo.
- Include a simple README file with instructions on how to start the app locally.
- Keep it simple for yourselves as always. Spend no more than 5 hours on this mini project.

### Prerequisites

- Node.js / npm

### Add these Installation instructions to your README

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/pizza-orders-api.git
    cd pizza-orders-api
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Run the server:
    ```bash
    node index.js
    ```

The server will run on `http://localhost:3000`.

## API Endpoints
### Order Model

```json
{
  "id": 1,
  "customerName": "Scott Tiger",
  "pizzaType": "Margherita",
  "extraToppings": ["cheese", "mushroom", "tomato"],
  "quantity": 1,
  "drink": "Coke",
  "status": "new"
}
```

- **Get all orders**: `GET /orders`
  - You can also filter orders by status: `GET /orders?status=new`

- **Create a new order**: `POST /orders`
- **Update an order**: `PUT /orders/:id`
- **Delete an order**: `DELETE /orders/:id`

## Git Branching Instructions

1. **Create your first feature branch**:
    ```bash
    git checkout -b feature/get-orders-endpoint
    ```

2. **Write your code to implement this API endpoint**.
3. **Test your code locally using Postman**.
4. **Merge your branch to main branch**:
    ```git checkout main
    git merge feature/add-order-endpoint
    ```
5. **Create your second feature branch from the main branch**:
    ```bash
    git checkout main
    git checkout -b feature/create-order-endpoint
    ```
6. **Write your code to implement this API endpoint**.
10. **Follow the same steps as you did for the previous feature** (i.e. test and merge to main branch).

## Contributing
  ### Other developers who are keen to contribbute to this repository should refer to the instructions below
1. Fork the repository.
2. Create your feature branch:
    ```bash
    git checkout -b feature/your-feature
    ```
3. Commit your changes:
    ```bash
    git commit -m 'Add some feature'
    ```
4. Push to the branch:
    ```bash
    git push origin feature/your-feature
    ```
5. Open a pull request.

## License

This project is licensed under the MIT License.
