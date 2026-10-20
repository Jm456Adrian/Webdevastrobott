# 🚀 Space Bot API Investigation Sheet

**Total Marks: 40**  
**TASK 1: Collect Required API Documentation**

This investigation sheet helps you gather key technical information from the three APIs required for the Space Bot project: **Webex Messaging API**, **ISS Current Location API**, **Weather API** and a **Geocoding API** , plus the Python time module. Also furhter investigate the application of Web Architecture and MVC design pattern in development of the Bot

---

##  Webex Messaging API (4 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `___________https://webexapis.com____________________` |
| Authentication Method | `__________________Bearer Authentication method_____________` |
| Endpoint to list rooms | `____________'/v1/rooms/'___________________` |
| Endpoint to get messages | `______________'/v1/messages/_________________` |
| Endpoint to send message | `________________'/v1/messages/'_______________` |
| Required headers | `__________''Authorization: Bearer (Token Here)'', 'Content-Type: application/json', 'Accept: application/json'_____________________` |
| Sample full GET or POST request | `__request('GET',https://webexapis.com/v1/rooms/?= , headers=headers, data = payload)_____________________________` |

---   {
    "items": [
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOmV1LWNlbnRyYWwtMV9rL1JPT00vMjdmZTZlZjAtYzdiNS0xMWYxLTk5MGItYzlkZDYxMGFjYjM1",
            "title": "Webt",
            "type": "group",
            "lastActivity": "2026-10-14T09:53:49.919Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS9hNTNjYmQ2OC05NzllLTQ0MTItOGU5My0yMjM1YTlmMjg0MDc",
            "created": "2026-10-14T09:53:49.919Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9jMThlMTNhZS01NTc1LTRiYzAtYWUwMS1lNDg5MDVmMTRmMTc",
            "isPublic": false,
            "isReadOnly": false,
            "isLocked": false
        },
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOmV1LWNlbnRyYWwtMV9rL1JPT00vMWQ0MjJjNDAtYzdiNS0xMWYxLTk5MGItYzlkZDYxMGFjYjM1",
            "title": "ISS",
            "type": "group",
            "lastActivity": "2026-10-14T09:53:31.908Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS9hNTNjYmQ2OC05NzllLTQ0MTItOGU5My0yMjM1YTlmMjg0MDc",
            "created": "2026-10-14T09:53:31.908Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9jMThlMTNhZS01NTc1LTRiYzAtYWUwMS1lNDg5MDVmMTRmMTc",
            "isPublic": false,
            "isReadOnly": false,
            "isLocked": false
        },
        {
            "id": "Y2lzY29zcGFyazovL3VybjpURUFNOmV1LWNlbnRyYWwtMV9rL1JPT00vMTc5OTgwZTAtYzdiNS0xMWYxLTliODUtY2JjMWRkMjJiYmQ1",
            "title": "Welcome space",
            "type": "group",
            "lastActivity": "2026-10-14T09:53:22.976Z",
            "creatorId": "Y2lzY29zcGFyazovL3VzL1BFT1BMRS9hNTNjYmQ2OC05NzllLTQ0MTItOGU5My0yMjM1YTlmMjg0MDc",
            "created": "2026-10-14T09:53:22.414Z",
            "ownerId": "Y2lzY29zcGFyazovL3VzL09SR0FOSVpBVElPTi9jMThlMTNhZS01NTc1LTRiYzAtYWUwMS1lNDg5MDVmMTRmMTc",
            "isPublic": false,
            "isReadOnly": false,
            "isLocked": false
        }
    ]
}

##  ISS Current Location API (2 marks)

| Criteria | Details |
|---------|---------|
| API Base URL | `_____________"http://api.open-notify.org"__________________` |
| Endpoint for current ISS location | `"http://api.open-notify.org/iss-now.json` |
| Sample response format (example JSON) |  
```
{
  "message": "success", 
  "timestamp": UNIX_TIME_STAMP, 
  "iss_position": {
    "latitude": CURRENT_LATITUDE, 
    "longitude": CURRENT_LONGITUDE
  }
}
```
|

---

##  Geocoding API (4 marks)

| Criteria | Details |
|---------|---------|
| Provider used (Choose one) | **LocationIQ / Mapbox/ OpenWeatherMap other -provide detail** |
| API Base URL | `_______________"http://api.openweathermap.org"________________` |
| Endpoint for geocoding | `_______________"/geo/1.0/direct"________________` |
| Endpoint for reverse geocoding | `_______________"/geo/1.0/reverse"________________` |
| Authentication method | `____________"http://api.openweathermap.org/geo/1.0/direct?q=London&limit=5&appid={API key}"___________________` |
| Required query parameters | `_______________________________` |
| Sample request with latitude/longitude | `_______________________________` |
| Sample JSON response (formatted example) |  
```

```
|

---


##  Weather API (3 marks)

| Criteria | Details |
|---------|---------|
| API Provider (Choose one) | **OpenWeather, OpenWeatherMap (or other – provide details)** |
| API Base URL | `_______________________________` |
| Endpoint for current weather | `_______________________________` |
| Authentication method | `_______________________________` |
| Required query parameters | `_______________________________` |
| Sample JSON response (formatted example) |  
```

```
|

---

##  Epoch to Human Time Conversion (Python time module) (2 marks)

| Criteria | Details |
|---------|---------|
| Library used | `_______________________________` |
| Function used to convert epoch | `_______________________________` |
| Sample code to convert timestamp |  
```  
```
|
| Output (human-readable time) | `_______________________________` |

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
