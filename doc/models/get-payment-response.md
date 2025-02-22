
# Get Payment Response

Defines the response returned by [GetPayment](/doc/api/payments.md#get-payment).

## Structure

`Get Payment Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `errors` | [`List of Error`](/doc/models/error.md) | Optional | Information about errors encountered during the request. |
| `payment` | [`Payment`](/doc/models/payment.md) | Optional | Represents a payment processed by the Square API. |

## Example (as JSON)

```json
{
  "payment": {
    "amount_money": {
      "amount": 200,
      "currency": "USD"
    },
    "app_fee_money": {
      "amount": 10,
      "currency": "USD"
    },
    "approved_money": {
      "amount": 200,
      "currency": "USD"
    },
    "card_details": {
      "auth_result_code": "nsAyY2",
      "avs_status": "AVS_ACCEPTED",
      "card": {
        "bin": "411111",
        "card_brand": "VISA",
        "card_type": "DEBIT",
        "exp_month": 7,
        "exp_year": 2026,
        "fingerprint": "sq-1-TpmjbNBMFdibiIjpQI5LiRgNUBC7u1689i0TgHjnlyHEWYB7tnn-K4QbW4ttvtaqXw",
        "last_4": "1111",
        "prepaid_type": "PREPAID"
      },
      "card_payment_timeline": {
        "authorized_at": "2019-07-10T13:23:49.234Z",
        "captured_at": "2019-07-10T13:23:49.446Z"
      },
      "cvv_status": "CVV_ACCEPTED",
      "entry_method": "ON_FILE",
      "statement_description": "SQ *MY MERCHANT",
      "status": "CAPTURED"
    },
    "created_at": "2019-07-10T13:23:49.154Z",
    "customer_id": "RDX9Z4XTIZR7MRZJUXNY9HUK6I",
    "id": "GQTFp1ZlXdpoW4o6eGiZhbjosiDFf",
    "location_id": "XTI0H92143A39",
    "note": "Brief description",
    "order_id": "m2Hr8Hk8A3CTyQQ1k4ynExg92tO3",
    "processing_fee": [
      {
        "amount_money": {
          "amount": 36,
          "currency": "USD"
        },
        "effective_at": "2019-07-10T15:23:49.000Z",
        "type": "INITIAL"
      }
    ],
    "receipt_number": "GQTF",
    "receipt_url": "https://squareup.com/receipt/preview/GQTFp1ZlXdpoW4o6eGiZhbjosiDFf",
    "reference_id": "123456",
    "source_type": "CARD",
    "status": "COMPLETED",
    "total_money": {
      "amount": 200,
      "currency": "USD"
    },
    "updated_at": "2019-07-10T13:23:49.446Z",
    "version_token": "hj8JqHWu9R1Kkfu63UuIUmYc7zm6YFOt92g8d2fb9fz6o"
  }
}
```

