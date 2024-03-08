
---

# Internet Computer Fish Market

This project is a demonstration of an Internet Computer application for managing a fish market. It allows users to add, remove, buy, and sell fishes through interactions with two canisters: `fishBase` for managing fishes and `payment` for handling payments.

## Features

- **Add Fish**: Add a new type of fish to the market with specified quantity and price.
- **Remove Fish**: Remove a type of fish from the market by its index.
- **List Available Fishes**: View the list of available fishes in the market.
- **Buy Fish**: Purchase a specified quantity of a fish from the market after authentication and payment.
- **Sell Fish**: Sell a specified type of fish to the market.

## Prerequisites

Before running the application, ensure you have the following installed:

- Node.js
- npm (Node Package Manager)

## Getting Started

1. Clone this repository to your local machine.
2. Install dependencies by running `npm install`.
3. Run the application using `npm start`.

## Usage

```typescript
// Example usage:

(async () => {
  await addFish({ name: 'Salmon', quantity: 10, price: 5 });
  await addFish({ name: 'Trout', quantity: 15, price: 7 });
  await listAvailableFishes();
  await buyFish('admin', 'password', 1, 5);
  await listAvailableFishes();
  await sellFish({ name: 'Tuna', quantity: 8, price: 10 });
})().catch((error) => {
  console.error('Error:', error);
});
```

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs, feature requests, or improvements.



