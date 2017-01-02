# flight-scanner
Track flights between destinations and alert the user of low prices.

Uses Google's QPX API. Inspired by https://github.com/ezekg/swa-dashboard

## Usage
```bash
export GOOGLE_QPX_API_KEY=""
```


### Twilio integration
If you have a Twilio account (I'm using a free trial account) and you've set up
a deal price threshold, you can set the following environment vars to set up SMS
deal alerts. _Just be warned: as long as the deal threshold is met, you're going
to receive SMS messages at the rate of the interval you defined. Better wake up
and book those tickets!_

```bash
export TWILIO_ACCOUNT_SID=""
export TWILIO_AUTH_TOKEN=""
export TWILIO_PHONE_FROM=""
export TWILIO_PHONE_TO=""
```
