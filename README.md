# SmartLogistics


## GPS tracking System <br/>

content <br/>
- Microcontroller stream to cloud

## send data from u-controller to mongoDB <br>
### Step 1: Setup Account<br>

![image](https://github.com/wanasyraf4/SmartLogistics/assets/107595740/086dedd8-ffd0-4408-b7aa-ef974b4c67a3) <br>

i. Go to mongodb.com and create a free account <br>
ii. Enable Data API in your account <br> 


![image](https://github.com/wanasyraf4/SmartLogistics/assets/107595740/828e858a-bfda-4d7b-b02f-56c9fead77cc) <br>

iii. Step through and generate an API Key, you will need to save the API key along with the URL they give you so you can access the cluster through an API call with the Raspberry Pi Pico W. <br>

![image](https://github.com/wanasyraf4/SmartLogistics/assets/107595740/c4e94729-8a71-44f6-9a2d-fc32c552830b)

iv. Create a database and collection in the UI, this is where we will store our example document. <br>

### Step 2: Code on Raspberry Pi Pico W

>egress.py

> note:
> Insert your internet name, internet password, MongoDB Data API URL, and API Key accordingly in the code. <br>
> In the payload you need to add your cluster, database, and collection names. <br>
> We are simply connecting to WiFi and sending a payload to their API with extension /action/insertOne, which will allow us to insert one document. We are using some dummy data for this example!
