Flight Tracker Application

This is a simple Flight Tracker web application built using Flask. The app allows users to track flights in real-time, providing departure/arrival information, flight status, and a map displaying flight paths. The app uses APIs to fetch flight data and geographical data for airport locations. 

```
Example of number: DL202, UA303, AA123 ...
Live demo https://flight-tracker-vercel-eliezersunny-eliezersunnys-projects.vercel.app/
```

Features

Flight Search: Search for a flight using its flight number.

Flight Information: Displays flight status, departure/arrival times, and airport information.

Flight Status: Displays whether the flight is active, delayed, or landed.

Map: Displays a map showing departure and arrival airport locations using Leaflet.js.


Tech Stack

Backend: Flask (Python)

API: AviationStack API for flight data, OpenCage API for geolocation data

Frontend: HTML, CSS (using Leaflet for the map display)

Deployment: Vercel (Serverless)


Installation

1. Clone the Repository:

``` bash
git clone https://github.com/EliezerSunny/Flight-tracker-vercel.git

cd Flight-tracker-vercel
```

2. Set up a Virtual Environment (Optional but recommended):

``` Window

# For Windows
python -m venv venv
.\api\Scripts\activate
```

``` MacOS/Linux
# For MacOS/Linux
python3 -m venv venv
source api/bin/activate
```

3. Install Dependencies:

```
pip install -r requirements.txt
```

4. Run the Flask Application:

Start the development server:

```
python api/app.py
```

Alternatively, you can use Gunicorn to run the app in a production-like environment:

```
gunicorn api.app:app
```


5. Access the Application:

Open a browser and visit http://127.0.0.1:5000/ to view the application locally.




Deployment on Vercel

To deploy the app on Vercel:

1. Create a Vercel Account: If you don’t have a Vercel account, create one at Vercel.


2. Install Vercel CLI:

```
npm install -g vercel
```

3. Deploy the Application:

In the root of the project directory, run the following command:

```
vercel
```
Follow the prompts to deploy your application.



4. Access the Deployed App:

After deployment, Vercel will provide a URL where your app is hosted.




Configuration

Make sure to replace the API keys in the api/app.py file:
```
AviationStack API Key: Replace API_KEY with your actual API key from AviationStack.
```

```
OpenCage API Key: Replace OPENCAGE_API_KEY with your OpenCage API key from OpenCage.
```

``` Project Structure

flight-tracker/
├── api/
│   └── app.py         # Flask app
├── static/
│   └── style.css      # CSS for styling
├── templates/
│   └── index.html     # HTML template for rendering flight info
├── requirements.txt   # List of dependencies
├── vercel.json        # Vercel configuration
└── README.md          # Project documentation
```

Dependencies

Flask: Micro web framework for Python.

Requests: HTTP library for making requests to external APIs.

Gunicorn: WSGI HTTP server for running the app in production.


Install all dependencies by running:

pip install -r requirements.txt

Contributing

1. Fork the repository.


2. Create a new branch (git checkout -b feature-branch).


3. Make your changes.


4. Commit your changes (git commit -am 'Add new feature').


5. Push to your branch (git push origin feature-branch).


6. Open a Pull Request.



License

This project is licensed under the MIT License - see the LICENSE file for details.
