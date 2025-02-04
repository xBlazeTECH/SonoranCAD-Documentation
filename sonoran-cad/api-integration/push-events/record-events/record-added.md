---
description: The EVENT_RECORD_ADD is sent when a new record has been added in the CAD.
---

# Record Added

{% hint style="warning" %}
This push event requires the **pro **version of Sonoran CAD or higher.\
For more information, see our [pricing ](../../../../pricing/faq/)page.
{% endhint %}

### EVENT_RECORD_ADD

Note: This event will NOT be fired when adding a record via API, as your server is already aware of the record being added.

```javascript
{
  "key": "YOUR_API_KEY", // Authenticate legitimate event traffic
  "type": "EVENT_RECORD_ADD",
  "data": {
    "record": {} // Custom record object
  }
}
```

### Custom Record Object

The `record` object will contain the custom record object, in accordance with the record format below:

{% content-ref url="../../api-endpoints/general/custom-records/" %}
[custom-records](../../api-endpoints/general/custom-records/)
{% endcontent-ref %}

