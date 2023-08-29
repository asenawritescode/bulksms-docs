# BULK SMS API Documentation

## Important Information 
- Costs KES. 0.6 per sms
- Cost KES. 0.3 per Whatsapp Message
- The recipients in the Whatsapp APi only accepts the format "2547XXXXXXXX"

## Creating an account

### Request

- Method: POST
- URL: `https://bulk-sms-production.up.railway.app/api/v1/account/new`

#### Body
- Should be a Safaricom number.

```json
{
"phone": "07XXXXXXXX"
}
```

## Credit money to your account

### Request

- Method: POST
- URL: `https://bulk-sms-production.up.railway.app/api/v1/account/pay`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX",
"amount": 50
}
```

## Check your account balance

### Request

- Method: POST
- URL: `https://bulk-sms-production.up.railway.app/api/v1/account/balance`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX"
}
```

## Send an SMS message to one recipient

### Request

- Method: POST
- URL: `https://bulk-sms-production.up.railway.app/api/v1/sms/send`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX",
"message": "Hello there !",
"recipient": ["07XXXXXXXX"]
}
```

## Send an SMS message to many recipients

### Request

- Method: POST
- URL: `https://bulk-sms-production.up.railway.app/api/v1/sms/send`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX",
"message": "Hello there !",
"recipient": ["07XXXXXXXX", "07XXXXXXXX"]
}
```

## Send a Whatsapp message to one recipient

### Request

- Method: POST
- URL: `[https://bulk-sms-production.up.railway.app/api/v1/whatsapp/send](https://bulk-sms-production.up.railway.app/api/v1/whatsapp/send)`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX",
"message": "Hello there !",
"recipient": ["2547XXXXXXXX"]
}
```

## Send a Whatsapp message to many recipients

### Request

- Method: POST
- URL: `[https://bulk-sms-production.up.railway.app/api/v1/whatsapp/send](https://bulk-sms-production.up.railway.app/api/v1/whatsapp/send)`

#### Headers

- apikey: addyourapikeyhere

#### Body

```json
{
"phone": "07XXXXXXXX",
"message": "Hello there !",
"recipient": ["2547XXXXXXXX", "2547XXXXXXXX"]
}
```

## Side Notes
- Please note that the `addyourapikeyhere` value in the headers should be replaced with your actual API key, the phone passed in the body should be a Safaricom number.

- I have added api collections for both Thunderclient and Postman, feel free to download and import them respectively.

- This documentation provides an overview of the available endpoints and their request details for the BULK SMS API.

- Let me know if you need any further assistance!
  **Ping me on asenasamson@gmail.com**

