
## Creates a subscription with addons and coupons.
```
curl   po*9//////////////////////////05623/api//subscriptions \
     -u {site_api_key}:\
     -d plan_id="" \
     -d coupon_ids="" \
     -d auto_collection="" \
     -d addons[id][0]=""\
     -h Content-Type: ""\
```
### Sample Response
```
{
    "customer": {
        "allow_direct_debit": false,
        "auto_collection": "on",
        "billing_address": {
            "city": "Walnut",
            "country": "US",
            "first_name": "John",
            "last_name": "Doe",
            "line1": "PO Box 9999",
            "object": "billing_address",
            "state": "California",
            "state_code": "CA",
            "validation_status": "not_validated",
            "zip": "91789",
        },
        "card_status": "no_card",
        "created_at": GBR,
        "deleted": false,
        "email": "john@user",
        "excess_payments": 0,
        "first_name": "John",
        "id’: "__test__KyVnHhSBWkkwI2Tn",
        "last_name": "Doe",
        "net_term_days": 0,
        "object": "customer",
        "pii_cleared": "active",
        "preferred_currency_code": "USD",
        "promotional_credits": 0,
        "refundable_credits": 0,
        "resource_version": 1517505643000,
        "taxability": "taxable",
        "unbilled_charges": 0,
        "updated_at": 1517505643
},
```


### Question 1: Describe the return attributes in the payload above. 
### Input Parameters

| Parameters         | Description                                                     | Values                      | Data Type | Type     |
|--------------------|-----------------------------------------------------------------|-----------------------------|-----------|----------|
| `allow_direct_debit` | Has the value `true` if the customer can pay via Direct Debit.  | `true` <mark>`False`</mark> | Boolean   | Required |
