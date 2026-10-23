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
| Required query parameters | `___________"q (location name), appid (API key), lat (latitude), lon (longitude),, appid (API key)"____________________` |
| Sample request with latitude/longitude | `_______"http://api.openweathermap.org/geo/1.0/reverse?lat=51.5098&lon=-0.1180&limit=5&appid={API key}"________________________` |
| Sample JSON response (formatted example) |  
```
[
    {
        "name": "London",
        "local_names": {
            "os": "Лондон",
            "bm": "London",
            "is": "Lundúnir",
            "ab": "Лондан",
            "he": "לונדון",
            "cy": "Llundain",
            "bn": "লন্ডন",
            "mr": "लंडन",
            "gv": "Lunnin",
            "io": "London",
            "sk": "Londýn",
            "ro": "Londra",
            "uz": "London",
            "hy": "Լոնդոն",
            "bi": "London",
            "mk": "Лондон",
            "lo": "ລອນດອນ",
            "br": "Londrez",
            "ce": "Лондон",
            "ln": "Londoni",
            "ba": "Лондон",
            "te": "లండన్",
            "tk": "London",
            "bo": "ལོན་ཊོན།",
            "kl": "London",
            "st": "London",
            "ascii": "London",
            "ta": "இலண்டன்",
            "zu": "ILondon",
            "ka": "ლონდონი",
            "am": "ለንደን",
            "su": "London",
            "feature_name": "London",
            "sv": "London",
            "vi": "Luân Đôn",
            "fa": "لندن",
            "kw": "Loundres",
            "cv": "Лондон",
            "eo": "Londono",
            "ky": "Лондон",
            "ne": "लन्डन",
            "pa": "ਲੰਡਨ",
            "cs": "Londýn",
            "sa": "लन्डन्",
            "ny": "London",
            "hi": "लंदन",
            "ku": "London",
            "zh": "倫敦",
            "mg": "Lôndôna",
            "om": "Landan",
            "bg": "Лондон",
            "la": "Londinium",
            "wo": "Londar",
            "pt": "Londres",
            "ca": "Londres",
            "ps": "لندن",
            "fo": "London",
            "ha": "Landan",
            "si": "ලන්ඩන්",
            "tg": "Лондон",
            "so": "London",
            "my": "လန်ဒန်မြို့",
            "sl": "London",
            "sn": "London",
            "uk": "Лондон",
            "be": "Лондан",
            "fj": "Lodoni",
            "tt": "Лондон",
            "fi": "Lontoo",
            "sq": "Londra",
            "ja": "ロンドン",
            "gl": "Londres",
            "yi": "לאנדאן",
            "av": "Лондон",
            "ay": "London",
            "ug": "لوندۇن",
            "en": "London",
            "ig": "London",
            "lv": "Londona",
            "ff": "London",
            "cu": "Лондонъ",
            "sr": "Лондон",
            "ru": "Лондон",
            "gu": "લંડન",
            "eu": "Londres",
            "an": "Londres",
            "sd": "لنڊن",
            "es": "Londres",
            "fr": "Londres",
            "bs": "London",
            "ga": "Londain",
            "co": "Londra",
            "tl": "Londres",
            "id": "London",
            "af": "Londen",
            "gd": "Lunnainn",
            "nl": "Londen",
            "ur": "لندن",
            "qu": "London",
            "rm": "Londra",
            "ml": "ലണ്ടൻ",
            "wa": "Londe",
            "ms": "London",
            "sm": "Lonetona",
            "el": "Λονδίνο",
            "lb": "London",
            "km": "ឡុងដ៍",
            "tw": "London",
            "fy": "Londen",
            "gn": "Londye",
            "et": "London",
            "tr": "Londra",
            "oc": "Londres",
            "mi": "Rānana",
            "az": "London",
            "kk": "Лондон",
            "to": "Lonitoni",
            "ee": "London",
            "mn": "Лондон",
            "sh": "London",
            "ht": "Lonn",
            "no": "London",
            "mt": "Londra",
            "hr": "London",
            "ar": "لندن",
            "de": "London",
            "yo": "Lọndọnu",
            "bh": "लंदन",
            "it": "Londra",
            "lt": "Londonas",
            "ko": "런던",
            "da": "London",
            "jv": "London",
            "or": "ଲଣ୍ଡନ",
            "hu": "London",
            "kv": "Лондон",
            "sc": "Londra",
            "th": "ลอนดอน",
            "se": "London",
            "li": "Londe",
            "nn": "London",
            "kn": "ಲಂಡನ್",
            "na": "London",
            "pl": "Londyn",
            "sw": "London"
        },
        "lat": 51.5074456,
        "lon": -0.1277653,
        "country": "GB",
        "state": "England"
    }
]
```
|

---


##  Weather API (3 marks)

| Criteria | Details |
|---------|---------|
| API Provider (Choose one) | OpenWeather |
| API Base URL | `______________openweathermap.org_________________` |
| Endpoint for current weather | `_______________GET /weather________________` |
| Authentication method | `_______________Token API________________` |
| Required query parameters | `____________lat, long, appid, (units, lang which is optional)___________________` |
| Sample JSON response (formatted example) |  
```
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
|

---

##  Epoch to Human Time Conversion (Python time module) (2 marks)

| Criteria | Details |
|---------|---------|
| Library used | `__________________datetime_____________` |
| Function used to convert epoch | `___________datetime.fromtimestamp()____________________` |
| Sample code to convert timestamp |  
```
from datetime import datetime

epoch_time = 1613474400  # Replace with your epoch time

dt_object = datetime.utcfromtimestamp(epoch_time)
formatted_time = dt_object.strftime('%Y-%m-%d %H:%M:%S')
print(formatted_time) 
```
|
| Output (human-readable time) | `____________2021-02-16 11:20:00___________________` |

---

##  Extended Feature API ( 3 marks)

| Criteria | Details |
|---------|---------|
| API Provider | '___NASA APOD______' |
| API Base URL | `_________api.nasa.gov______________________` |
| Endpoint | `_____________/wp-json/wp-v2/apod-basic__________________` |
| Authentication method | `______________Token API_________________` |
| Required query parameters | `___________api_key (if not it uses DEMO KEY as default)____________________` |
| Sample JSON response (formatted example) |  
```
{
"date": "2026-09-11",
"post_id": 1308668,
"title": "M83: The Southern Pinwheel",
"permalink": "https://science.nasa.gov/image-article/apod-2026-september-11-m83-the-southern-pinwheel/",
"media_type": "image",
"explanation": "Detailed Explanation",
"credit": "Aldo Zanetti",
"copyright": "Aldo Zanetti",
"alt": "A spiral galaxy is shown in front of a dark field of stars.",
"url": "https://science.nasa.gov/image-article/apod-2026-september-11-m83-the-southern-pinwheel/",
"hdurl": "https://assets.science.nasa.gov/dynamicimage/assets/science/cds/apod/apod/2026/september/M83_Final2_1x.jpg?w=3828&h=3798&fit=clip&crop=faces%2Cfocalpoint",
"basic_html": "HTML of the page",
"basic_html_url": "https://science.nasa.gov/wp-json/wp/v2/apod-basic/260911/html"
}
```
|

--- 

##  Evaluation – Web Architecture, MVC Design & Security 

In this section, evaluate how web technologies, architecture, and design patterns have been applied in your **AstroBot**. Your responses must relate directly to your implementation and include reflection on your design decisions.

---

###  Web Architecture – Client–Server Model (3 marks)

Explain how the client–server model applies to your AstroBot:

- Identify the **client**      AstroBot Application (Python Script): Acts as an HTTP client that initiates requrests to external web APIs to retrieve data and publish messages. Webex Client App: Acts as the user interface client where the end-user inputs commands and views outputs.
- Identify the **server(s)**  Webex REST API Server.  Open-Notify API Server. Open-Meteo API Server   
- Describe how data flows between:
  - User, AstroBot and APIs.
    User Request: The user types a command (e.g., /weather London or /iss) into the Webex app.   Webex Polling: AstroBot sends a GET request to the Webex API server to read the latest message.   API Query: AstroBot parses the command and sends an HTTP GET request to the relevant third-party API server (OpenWeatherMap, Open-Notify, or Open-Meteo).   Data Response: The third-party API server returns a JSON response containing the requested raw data.   Message Delivery: AstroBot formats the JSON data into a readable text string and sends a POST request to the Webex API server, which displays the response in the user's Webex chat room. 

Include a **simple block diagram** to illustrate this interaction.

####  Security Considerations: (3 marks )
- Consider but not limiting to secure handling of API keys and tokens, API rate limiting, and Input validation (e.g., handling user commands safely), include examples from code where necessary to illustrate.
1. Secure Handling of API Keys and TokensRuntime User Input: Sensitive Webex tokens and OpenWeatherMap API keys are prompted securely at runtime via get_webex_token() and get_api_key() rather than being committed directly to public source control repositories.   Code Example:
   def get_webex_token():
   
   choice = input("Use hard-coded Webex token? (y/n): ").lower()
    if choice == "n":
        token = input("Enter your Webex Access Token: ")
        return f"Bearer {token}"


3. API Rate Limiting & Loop Polling ControlControlled Polling Delay: To avoid exceeding API rate limits or triggering HTTP 429 (Too Many Requests) throttling on Webex servers, the main polling loop enforces a mandatory 5-second sleep interval between polls.   Code Example:
   while True:
    # Process message logic...
    time.sleep(5)  # Enforces rate limiting compliance


5. Input Validation & Exception HandlingCommand & Parameter Validation: User commands are stripped and validated to prevent execution errors. Commands like /weather verify parameter count before issuing network requests to prevent IndexError exceptions.   Network Exception Guardrails: External API requests are wrapped with HTTP status checks (response.status_code == 200) and try-except blocks to handle network timeouts or server failures safely without crashing the bot runtime.   Code Example:
   parts = message_text.split(maxsplit=1)
	if len(parts) < 2:
    	send_message(token, room_id, "Usage: /weather <city>")
	else:
    	city = parts[1]
    	send_message(token, room_id, get_weather(city, weather_key))

---

###  RESTful API Usage in Your Application (3 marks )

Explain how REST APIs are used in your AstroBot: 

- Describe how HTTP methods (GET, POST) are used
  GET: Used to query data from remote servers without changing state. Used in requests.get() to retrieve rooms (/rooms), read latest messages (/messages), fetch weather metrics, and get ISS coordinates.   Pythonresponse = requests.get(url, headers=headers, params=params)
POST: Used to submit data payloads to remote servers. Used in send_message() with requests.post() to publish formatted bot replies to Webex chat rooms.   Pythonresponse = requests.post(url, headers=headers, data=json.dumps(data))
- Explain how your bot interacts with APIs (Webex, Weather, ISS, Geocoding)
Webex API: Monitors user messages in a specific room and posts command results back to the room.   OpenWeatherMap Direct Geocoding API: Converts city names from /weather <city> commands into exact latitude/longitude coordinates.   OpenWeatherMap Weather API: Takes coordinates to fetch current temperature, humidity, wind speed, and weather descriptions.   Open-Notify ISS API: Fetches the real-time orbital location of the Space Station.   OpenWeatherMap Reverse Geocoding API: Converts ISS raw coordinates into nearby country/city names. 
- Describe how JSON responses are received and processed
Responses are converted from raw JSON payloads into Python dictionary structures using response.json(). Specific data fields are safely extracted using dictionary keys and formatted into multi-line display strings.   Pythonweather = response.json()
temp = weather["main"]["temp"]
description = weather["weather"][0]["description"]

Note: Relate your explanation directly to your code for higher grade. 

#### Security Considerations: (2 marks)
- Check response status codes, Handling invalid or unexpected API responses, Avoiding excessive API calls
Status Code Checks: All API calls evaluate if response.status_code != 200: before attempting to parse JSON, returning error notices if an external API fails.   Pythonif response.status_code != 200:
    return "Error fetching weather data from OpenWeatherMap."
Handling Unexpected API Responses: try-except blocks wrap API calls to catch connectivity exceptions, and .get() statements safely query optional JSON fields without throwing key errors.   Pythonplace = f"{location.get('name', 'Unknown')}, {location.get('country', '')}"
Avoiding Excessive API Calls: A mandatory 5-second sleep timer (time.sleep(5)) is included inside the continuous polling loop to stay within API rate limit rules and prevent HTTP 429 throttling.   Pythonwhile True:
    # Polling and message logic...
    time.sleep(5)
---

###  MVC Design Pattern in AstroBot (3 Marks)

Explain how the **Model–View–Controller (MVC)** pattern applies to your solution:
Provide a short example based on your implementation

| Component   | Description and Example (Relate to your Bot) |
|------------|----------------------------------|
| **Model**  |**Description:** Manages raw data fetching, processing, and application business logic.<br>**Example:** Data functions like `get_weather()`, `get_iss_location()`, and `get_astronomy_info()` perform external HTTP requests, parse raw JSON data, and manage logical data structures.  |
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
