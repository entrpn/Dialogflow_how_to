# Dialogflow_how_to

### How to run ngrok

- Run function from the function folder

firebase --project <project_id> serve --only functions

- This will give you a local url. Ex:

✔  functions: dialogflowFirebaseFulfillment: http://localhost:5000/ces-2019-81670/us-central1/dialogflowFirebaseFulfillment

- On another console launch ngrok with the port from above:

ngrok http 5000

- This is the url you get back:

```
Session Status                online                                                                                                    
Session Expires               7 hours, 59 minutes                                                                                       
Version                       2.2.8                                                                                                     
Region                        United States (us)                                                                                        
Web Interface                 http://127.0.0.1:4040                                                                                     
Forwarding                    http://30cc39e0.ngrok.io -> localhost:5000                                                                
Forwarding                    https://30cc39e0.ngrok.io -> localhost:5000                                                               
                                                                                                                                        
Connections                   ttl     opn     rt1     rt5     p50     p90                                                               
                              0       0       0.00    0.00    0.00    0.00 
```

- Go on the dialogflow console and update the fullfillment as such

https://3334f350.ngrok.io/ces-2019-81670/us-central1/dialogflowFirebaseFulfillment
