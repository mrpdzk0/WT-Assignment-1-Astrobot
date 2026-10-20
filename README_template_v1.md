# 🚀 Space Bot API Investigation Sheet

**Total Marks: 40**  
**TASK 1: Collect Required API Documentation**

This investigation sheet helps you gather key technical information from the three APIs required for the Space Bot project: **Webex Messaging API**, **ISS Current Location API**, **Weather API** and a **Geocoding API** , plus the Python time module. Also furhter investigate the application of Web Architecture and MVC design pattern in development of the Bot

---

##  Webex Messaging API (4 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `_______________________________` |
| Authentication Method | `_______________________________` |
| Endpoint to list rooms | `_______________________________` |
| Endpoint to get messages | `_______________________________` |
| Endpoint to send message | `_______________________________` |
| Required headers | `_______________________________` |
| Sample full GET or POST request | `_______________________________` |

---

##  ISS Current Location API (2 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `http://api.open-notify.org/iss-now.json` |
| Endpoint for current ISS location | `{"timestamp": 1790251802, "iss_position": {"latitude": "-45.2251", "longitude": "-71.4836"}, "message": "success"}` |
| Sample response format (example JSON) |

'{
  "timestamp": 1790251802,
  "iss_position": {
    "latitude": "-45.2251",
    "longitude": "-71.4836"
  },
  "message": "success"
}'

```
|

---

##  Geocoding API (4 marks)

| Criteria | Details |
|---------|---------|
| Provider used (Choose one) |OpenWeatherMap - 5006dd63035cee6fdb48e0ea65892341|
| API Base URL | `https://openweathermap.org/` |
| Endpoint for geocoding | `_______________________________` |
| Endpoint for reverse geocoding | `_______________________________` |
| Authentication method | `appid={API key}` |
| Required query parameters | `_______________________________` |
| Sample request with latitude/longitude | `_______________________________` |
| Sample JSON response (formatted example) |  
{
  "lat": 51.5,
  "lon": -0.1,
  "timezone": "Europe/London",
  "timezone_offset": 3600,
  "data": [
    {
```

```
|

---


##  Weather API (3 marks)

| Criteria | Details |
|---------|---------|
| API Provider (Choose one) |OpenWeatherMap - 5006dd63035cee6fdb48e0ea65892341££|
| API Base URL | `_______________________________` |
| Endpoint for current weather | `_______________________________` |
| Authentication method | `appid={API key}` |
| Required query parameters | `_______________________________` |
| Sample JSON response (formatted example) |  
{
  "lat": 51.5,
  "lon": -0.1,
  "timezone": "Europe/London",
  "timezone_offset": 3600,
  "data": [
    {
      "dt": 1777449371,
      "sunrise": 1777437375,
      "sunset": 1777490344,
      "temp": 286.42,
      "feels_like": 285.32,
      "pressure": 1024,
      "humidity": 58,
      "dew_point": 278.34,
      "uvi": 1.55,
      "clouds": 0,
      "visibility": 10000,
      "wind_speed": 8.23,
      "wind_deg": 70,
      "weather": [
        {
          "id": 800,
          "main": "Clear",
          "description": "sky is clear",
          "icon": "01d"
        }
      ]
	  "alerts": [
		"8B46C632-DCA7-44D7-8BDF-02445621BAFF",
		"29F58A35-BB91-4A73-9F46-9FC64BDF604F",
		...
	]
    }
  ]
}
```

```
|

---

##  Epoch to Human Time Conversion (Python time module) (2 marks)

| Criteria | Details |
|---------|---------|
| Library used | `time` |
| Function used to convert epoch | `_______________________________` |
| Sample code to convert timestamp |  

'import time

epoch_time = 1613474400  # Replace with your epoch time

formatted_time = time.strftime('%Y-%m-%d %H:%M:%S', time.gmtime(epoch_time))
print(formatted_time)'

```  
```
|
| Output (human-readable time) | `2021-02-16 11:20:00` |

---

##  Extended Feature API ( 3 marks)

| Criteria | Details |
|---------|---------|
| API Provider | '_________' |
| API Base URL | `_______________________________` |
| Endpoint | `_______________________________` |
| Authentication method | `_______________________________` |
| Required query parameters | `_______________________________` |
| Sample JSON response (formatted example) |  
```

```
|

--- 

##  Evaluation – Web Architecture, MVC Design & Security 

In this section, evaluate how web technologies, architecture, and design patterns have been applied in your **AstroBot**. Your responses must relate directly to your implementation and include reflection on your design decisions.

---

###  Web Architecture – Client–Server Model (3 marks)

Explain how the client–server model applies to your AstroBot:

- Identify the **client** 
- Identify the **server(s)** 
- Describe how data flows between:
  - User, AstroBot and APIs

Include a **simple block diagram** to illustrate this interaction.

####  Security Considerations: (3 marks )
- Consider but not limiting to secure handling of API keys and tokens, API rate limiting, and Input validation (e.g., handling user commands safely), include examples from code where necessary to illustrate.

---

###  RESTful API Usage in Your Application (3 marks )

Explain how REST APIs are used in your AstroBot: 

- Describe how HTTP methods (GET, POST) are used  
- Explain how your bot interacts with APIs (Webex, Weather, ISS, Geocoding)  
- Describe how JSON responses are received and processed  

Note: Relate your explanation directly to your code for higher grade. 

#### Security Considerations: (2 marks)
- Check response status codes, Handling invalid or unexpected API responses, Avoiding excessive API calls

---

###  MVC Design Pattern in AstroBot (3 Marks)

Explain how the **Model–View–Controller (MVC)** pattern applies to your solution:
Provide a short example based on your implementation

| Component   | Description and Example (Relate to your Bot) |
|------------|----------------------------------|
| **Model**  |  |
| **View**   |  |
| **Controller** |  |

---

### 📝 Reflection and Evaluation ( 8 marks )

Reflect on your AstroBot (400 words):

- How effective is your bot in meeting the Astronomy Club’s needs?  
- What design decisions worked well?  
- What challenges did you face when integrating APIs?  
- What security risks did you identify and how were they handled?  
- How could your solution be improved in the future?  

---

 **Tip:** Link your answers directly to your code and examples for higher marks.
### Notes

- Use official documentation for accuracy (e.g. developer.webex.com, locationiq.com or Mapbox, open-notify.org or other ISS API).
- Be prepared to explain your findings to your instructor or demo how you retrieved them using tools like Postman, Curl, or Python scripts.

---

###  Total: /40