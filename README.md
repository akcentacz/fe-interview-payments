# Front-end developer interview

## Payments overview application

### Task for the React/Next.js Developer Candidate

**Project: Payment Overview Page**

#### Goal:
Create an interactive web application that displays a list of payments, allows navigation to payment details, and provides filtering and sorting functionalities.

#### Requirements:
1. **Functionality**:
    - Display a list of payments in a table or card format with the following data:
        - Payment Date
        - Amount
        - Currency (USD, EUR, CZK, HUF)
        - Payment Type (BANK_TRANSFER, APPLE_PAY, GOOGLE_PAY, CARD_ONLINE)
        - Payment Status (PENDING, SUCCESS, CANCELED)
    - Implement a link/button to payment details that shows the following information:
        - Payment Date + Time
        - Amount
        - Currency
        - Payment Type
        - Payment Status
        - Payment Recipient
        - Formatted Note
    - Add filtering options based on various criteria (e.g., date, amount, payment type).
    - Enable sorting of payments by different columns (e.g., date ascending/descending, amount ascending/descending).
    - Allow the use of any necessary libraries.

2. **Technology**:
    - Use React.js/Next.js.
    - TypeScript is preferred.
    - Styling is up to you. You can use any CSS framework or write your own styles.

#### Additional Information:
- The payment overview data is located in the file `data/payments/index.json` and can be fetched directly from the following URL:
  "https://raw.githubusercontent.com/akcentacz/fe-interview-payments/refs/heads/main/data/payments/index.json"
- The payment details are located in individual files under
  `data/payments/details/{paymentId}.json` and can be fetched directly from a URL,
  for example,
  "https://raw.githubusercontent.com/akcentacz/fe-interview-payments/refs/heads/main/data/payments/details/1.json" or
  "https://raw.githubusercontent.com/akcentacz/fe-interview-payments/refs/heads/main/data/payments/details/19.json"
- If the payment detail file does not exist, the response should handle HTTP status code 404 appropriately.
- We prefer the completed task to be shared as a link to a public GitHub repository.