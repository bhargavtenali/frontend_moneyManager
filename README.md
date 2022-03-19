In this project, let's build a **Money Manager** app by applying the concepts we have learned till now.

### Refer to the image below:

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/money-manager-output.gif" alt="money manager output gif" style="max-width:70%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Extra Small (Size < 576px) and Small (Size >= 576px)](https://assets.ccbp.in/frontend/content/react-js/money-manager-sm-output-v2.png)
- [Medium (Size >= 768px), Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/money-manager-lg-output.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- Initially, Balance Amount, Income Amount, and Expenses Amount should be `0`
- Balance Amount should be calculated by removing the Expenses Amount from the Income Amount in the list of transactions
- Income Amount should be calculated by removing the Expenses Amount in the list of transactions
- Expenses Amount should be calculated by adding only Expenses Amount in the list of transactions
- The `MoneyManager` component is provided with `transactionTypeOptions`. It consists of a list of transaction type objects with the following properties in each object

  |     Key     | Data Type |
  | :---------: | :-------: |
  |  optionId   |  String   |
  | displayText |  String   |

- Initially, the value of the `titleInput` should be empty
- Initially, the value of the `amountInput` should be empty
- Initially, the first option in the list should be selected
- When a transaction is added, by providing the values in the `titleInput`, `amountInput` and `optionId` and **Add** button is clicked,

  - A new transaction should be added to the transaction history list
  - `totalBalance`, `totalIncome` and `totalExpenses` should be updated accordingly

    ```
    totalBalance = totalIncome - totalExpenses
    ```

  - After updating, the values in the `titleInput`,`amountInput` and `optionId` will be updated to their initial values

- When the delete button in the transaction history is clicked,
  - The respective transaction should be deleted from the transaction history list
  - `totalBalance`, `totalIncome` and `totalExpenses` should be updated accordingly

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/money-manager-component-structure-breakdown.png" alt="component breakdown structure" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/App.js`
- `src/components/MoneyManager/index.js`
- `src/components/MoneyManager/index.css`
- `src/components/MoneyDetails/index.js`
- `src/components/MoneyDetails/index.css`
- `src/components/TransactionItem/index.js`
- `src/components/TransactionItem/index.css`
</details>

### Important Note

<details>
<summary>Click to view</summary>

<br/>

**The following instructions are required for the tests to pass**

- The Balance Amount should have the testid as **balanceAmount**
- The Income Amount should have the testid as **incomeAmount**
- The Expenses Amount should have the testid as **expensesAmount**
- The Delete button for each transaction should have the testid as **delete**

</details>

### Resources

<details>
<summary>Image URLs</summary>

- [https://assets.ccbp.in/frontend/react-js/money-manager/money-manager-bg.png](https://assets.ccbp.in/frontend/react-js/money-manager/money-manager-bg.png)
- [https://assets.ccbp.in/frontend/react-js/money-manager/balance-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/balance-image.png) alt should be **balance**
- [https://assets.ccbp.in/frontend/react-js/money-manager/income-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/income-image.png) alt should be **income**
- [https://assets.ccbp.in/frontend/react-js/money-manager/expenses-image.png](https://assets.ccbp.in/frontend/react-js/money-manager/expenses-image.png) alt should be **expenses**
- [https://assets.ccbp.in/frontend/react-js/money-manager/delete.png](https://assets.ccbp.in/frontend/react-js/money-manager/delete.png) alt should be **delete**

</details>

<details>
<summary>Colors</summary>

<br/>

<div style="background-color: #475569; width: 150px; padding: 10px; color: white">Hex: #475569</div>
<div style="background-color: #0b69ff; width: 150px; padding: 10px; color: white">Hex: #0b69ff</div>
<div style="background-color: #ecfccb; width: 150px; padding: 10px; color: black">Hex: #ecfccb</div>
<div style="background-color: #84cc16; width: 150px; padding: 10px; color: black">Hex: #84cc16</div>
<div style="background-color: #cffafe; width: 150px; padding: 10px; color: black">Hex: #cffafe</div>
<div style="background-color: #06b6d4; width: 150px; padding: 10px; color: black">Hex: #06b6d4</div>
<div style="background-color: #ede9fe; width: 150px; padding: 10px; color: black">Hex: #ede9fe</div>
<div style="background-color: #7c3aed; width: 150px; padding: 10px; color: white">Hex: #7c3aed</div>
<div style="background-color: #cbd5e1; width: 150px; padding: 10px; color: black">Hex: #cbd5e1</div>
<div style="background-color: #7e858e; width: 150px; padding: 10px; color: black">Hex: #7e858e</div>
<div style="background-color: #ffffff; width: 150px; padding: 10px; color: black">Hex: #ffffff</div>
<div style="background-color: #1e293b; width: 150px; padding: 10px; color: white">Hex: #1e293b</div>
<div style="background-color: #d7dfe9; width: 150px; padding: 10px; color: black">Hex: #d7dfe9</div>
<div style="background-color: #334155; width: 150px; padding: 10px; color: white">Hex: #334155</div>

</details>

<details>
<summary>Font-families</summary>

- Roboto

</details>

> ### _Things to Keep in Mind_
>
> - All components you implement should go in the `src/components` directory.
> - Don't change the component folder names as those are the files being imported into the tests.
> - **Do not remove the pre-filled code**
> - Want to quickly review some of the concepts you’ve been learning? Take a look at the Cheat Sheets.
