# PassportPayments Client Library in JS
The repository contains the client support library for [PassportPayments API](https://api.passportpayments.com/docs/) written in Javascript

## Usage

```js
<script type="text/javascript" src="https://s3.amazonaws.com/passportpayments/js/passportpayments-1.0.0.min.js"></script>
```

```js
var endPoint = "https://sandbox.passportpayments.com/index.php"
var pp = new PassportCardToken(APP_KEY, endPoint); // YOUR APPKEY

var params = {
    "cardnumber": '4111111111111111'
    "expmonth": '12',
    "expyear": '2020',
    "cvv": '123'
}
// params, successCallback, errorCallback, complete_response
  pp.getCardToken(params, cardTokenSuccess, cardTokenError, false);
```

