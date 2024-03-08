
---

# Internet Computer Fish Market

The Internet Computer Fish Market is a demonstration application showcasing the capabilities of the Internet Computer platform for managing a virtual fish market. This application allows users to interact with two canisters: `fishBase` for managing fishes and `payment` for handling payments. Users can perform various actions such as adding new fishes, removing fishes, buying fishes, and selling fishes.

## Features

### Add Fish

Users can add a new type of fish to the market with a specified quantity and price.

### Remove Fish

Users can remove a type of fish from the market by its index.

### List Available Fishes

Users can view the list of available fishes in the market, including their names, quantities, and prices.

### Buy Fish

Authenticated users can purchase a specified quantity of a fish from the market after making a payment.

### Sell Fish

Users can sell a specified type of fish to the market.

## Prerequisites

Before running the application, ensure you have the following installed:

- **Node.js:** You need Node.js to run the JavaScript code in this project.
- **npm (Node Package Manager):** npm is used to manage project dependencies.

## Getting Started

1. **Clone the Repository:** Clone this repository to your local machine using the following command:
   ```
   git clone https://github.com/your-username/internet-computer-fish-market.git
   ```

2. **Install Dependencies:** Navigate to the project directory and install dependencies by running:
   ```
   npm install
   ```

3. **Start the Application:** Run the application using:
   ```
   npm start
   ```

## Usage

```typescript
// Example usage:

(async () => {
  // Add fishes to the market
  await addFish({ name: 'Salmon', quantity: 10, price: 5 });
  await addFish({ name: 'Trout', quantity: 15, price: 7 });

  // List available fishes
  await listAvailableFishes();

  // Buy fishes from the market
  await buyFish('admin', 'password', 1, 5);

  // List available fishes after purchase
  await listAvailableFishes();

  // Sell fish to the market
  await sellFish({ name: 'Tuna', quantity: 8, price: 10 });
})().catch((error) => {
  console.error('Error:', error);
});
```

## Contributing

Contributions are welcome! If you have any ideas for improvements, bug fixes, or new features, please feel free to submit a pull request or open an issue. Your contributions help improve the project for everyone.


