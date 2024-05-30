# savings-demo

### Scenario

- Current banking customer want help apply for a Saving Account.
- Personas
    - Chris = Customer
    - Angi = Banking Support Agent
    - Paula = Process Owner
    - Codi = Developer
- Chris calls the bank’s customer support in while on iOS device
- Chris gets connected to Angi
- Angi is presented with a 360 view of Chris’ accounts, balances, notifications and any open ticket
    - Checking
    - Car Loan
    - Credit Card
- Angi initiates the Saving account application
- Chris receives email with application link
- Angi and Chris complete form together
- Chris uploads license for OCR details
- Angi notices that SSN is missing a validation

### Change Process

- Angi notifies Paula capturing SSN is missing from the process

> application.ssn
> 
- Paula adds a input field, label and adds data key
- Does not know how to add validation. Needs RegEx
- Works with Codi for RegEx to validate SSN
    - Pattern
        - (?!(\d){3}(-| |)\1{2}\2\1{4})(?!666|000|9\d{2})(\b\d{3}(-| |)(?!00)\d{2}\4(?!0{4})\d{4}\b)
- Clear cache

### Resume Saving Account Application

- Chris scans ID for SSN
    - Valid SSN: 457-55-5462
- Chris upload pay stub
- Both complete form and Chris receives email confirmation

### AI Example

- Use Oven to show AI form creation from samples below

### Features Covered

- Forms
- OCR
- Image upload
- Email
- Dynamic changes
- AI