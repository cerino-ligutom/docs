---
id: sending-requests
title: Sending Requests
hide_title: true
---

# Sending Requests

## Call the ```SuperTokensURLSession.dataTask``` method: [API Reference](./api-reference#supertokensurlsessiondatataskrequest-urlrequest-completionhandler-escaping-data-urlresponse-error-void)

```swift
import SuperTokensSession

let url = URL(string: "http://api.example.com/api/getUserInfo")
var request = URLRequest(url: url!)
request.httpMethod = "POST"
SuperTokensURLSession.dataTask(request: request, completionHandler: {
    data, response, error in

    // DO SOMETHING
})
```

- Unlike with ```URLSession```, you cannot suspend, resume and cancel tasks as of yet. In case this is required, please [contact us](mailto:team@supertokens.io)