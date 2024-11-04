# Receipt HTML

```html
<!-- receipt.html -->
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Receipt</title>
    <link rel="stylesheet" href="app.css" />
  </head>

  <body>
    <div class="print-button">
      <button onclick="printReceipt()" type="button">Print Receipt</button>
    </div>
    <main class="receipt-container">
      <div class="receipt-wrapper">
        <div class="header">
          <h1>Billing App</h1>
          <p>
            1234 Business St,<br />City, State, ZIP<br />Phone: (123) 456-7890
          </p>
        </div>
        <hr />
        <div class="customer-details">
          <p>Customer Mobile: <span id="customer-mobile"></span></p>
          <p>Date: <span id="receipt-date"></span></p>
          <p>Time: <span id="receipt-time"></span></p>
        </div>
        <hr />
        <div class="product-details">
          <table>
            <thead>
              <tr>
                <th>Product Name</th>
                <th>Price</th>
                <th>Qty</th>
                <th>Total</th>
              </tr>
            </thead>
            <tbody id="product-table-body">
              <!-- Product rows will be inserted here -->
            </tbody>
          </table>
        </div>
        <hr />
        <div class="total-amount">
          <p>Total Amount: ₹<span id="total-amount">0.00</span></p>
        </div>
        <div class="footer">
          <p>Thank you for your purchase!</p>
        </div>
      </div>
    </main>

    <script src="receipt.js"></script>
  </body>
</html>
```


# Receipt CSS

```css
/* receipt style  */
.receipt-container {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 50px 0;
}

.receipt-wrapper {
  background-color: #fff;
  padding: 20px;
  border-radius: 5px;
  border: 1px solid #eee;
}

.receipt-wrapper .header {
  text-align: center;
  margin-bottom: 10px;
}

.receipt-wrapper .header h1 {
  margin-bottom: 5px;
}

.receipt-wrapper .customer-details p {
  margin: 5px 0;
}

.receipt-wrapper .customer-details,
.receipt-wrapper .total-amount {
  margin: 10px 0;
}

.receipt-wrapper .product-details table {
  width: 100%;
  border-collapse: collapse;
}

.receipt-wrapper .product-details th,
.receipt-wrapper .product-details td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: left;
}

.receipt-wrapper .product-details th {
  background-color: #f2f2f2;
}

.receipt-wrapper .footer {
  text-align: center;
  margin-top: 20px;
}

.print-button {
  text-align: center;
  margin-top: 50px;
}

.print-button button {
  background-color: #f0db4f;
  border: none;
  outline: none;
  padding: 10px;
}
```
