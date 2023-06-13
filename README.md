# 🛠️ Tensor 🛠️
Tensor is a bank loan application service that lets customer apply for loan and the banker can either accept or decline the loan application.

### I. Overview
overview - Tensor is a bank loan application service that lets customers apply for loan and the banker can either accept or decline the loan application. This project uses the Proposal Accept design pattern. 


### II. Workflow
1. Customer creates a LoanApplication Contract
2. Customer is allowed to create only one LoanApplication contract at a time
3. The banker takes the contract and either approves the loan or rejects the loan
4. If the loan is approved, the banker creates the loan contract and assigns it to the customer
5. If the loan is rejected by the bank, the LoanApplication contract is archived
6. The customer can then get the option to pay back the loan by PayLoan choice in the Loan contract
7. The customer can Modify the loan contract by adding more money to the loan
8. If the customer pays back the loan, the loan contract is archived


### III. Compiling & Testing
To compile and test, run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml start
```
Upon using `daml start` the navigator will open up and you will be able to select a role of either "Banker" or "Customer"
