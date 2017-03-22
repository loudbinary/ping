# ping
Device Prototype #2

1. Configure limited use IAM Authentication Key.  
2. Assign key to device.
3. Boot Raspberry PI, start node script automatically
4. Script start

* Create NODE Package, npm init
* npm install dotenv --save
* npm install aws-sdk
* Create a .env file
* In file place DEVICEID=PING_SERVER
* Using AWS Credentials IN config.json
* Read in .env with instructions.
* Call simple register lambda, that responds with SNS - ARN
* Device subscribes to SNS ARN
* Waits for PING Message to be published into SNS Topic
* Upon PING, responds to PING with { type: PING, message: PING, DEVICEID: <deviceid>}
* Repeat
