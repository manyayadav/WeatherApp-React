## API Keys

### To get an API key from Google for this project:

1. Go to the Google Cloud Console: https://console.cloud.google.com/ and sign up.
2. Create e New Project.
3. Enable the required APIs. To do this, navigate to the "APIs & Services" > "Library" section in your project under the Maps category. For this application you'll need the Geolocation API and the Maps Static API.
4. Create Credentials: After enabling the necessary APIs, go to the "APIs & Services" > "Credentials" section. Click on the "Create Credentials" button and select "API Key."
5. Add Your API Key to Your Project: Once you've created and configured your API key, you'll receive the key value. You can now add this API key to your project's configuration. 

### To get an API Key from Open Weather:

1. Go to the OpenWeather Website: https://home.openweathermap.org/
2. Sign Up or Log In to access your Profile and services.
3. Click on your user name on the top right drop down and select "My API keys".
4. Click on the "Generate" button to generate a new API key. Once generated, your API key will be displayed on the screen. Copy the API key to use it in your project.
5. Read the documentation at https://openweathermap.org/api/one-call-3#current to learn how to make an API call. You can now add this API key to your project's configuration. 

### Use your API Keys

1. In the Home.jsx file replace the following:
   - Find ```export const WEATHER``` and reassign it to your weather API Key.
   - Find ```const geoURL = `https://www.googleapis.com/geolocation/v1/geolocate?key=${
    import.meta.env.VITE_MAP_API_KEY }`;``` and replace the information after "key=" with your Google API Key.
   - Find ```const staticURL = `https://maps.googleapis.com/maps/api/staticmap?center=${lat},${lon}&zoom=${zoom}&size=${size}&key=${
    import.meta.env.VITE_MAP_API_KEY
  }`;``` and replace the information after "key=" with your Google API Key.
2. In the BigMap.jsx replace the following:
   - Find ```const getMap = `https://www.google.com/maps/embed/v1/place?key=${
    import.meta.env.VITE_MAP_API_KEY
  }&q=${location}`;``` and replace the information after "key=" with your Google API Key.

  
-------------------------------------------------

## Installation

To run this project locally, follow these steps:

1. Clone the repository:

```bash
git clone https://github.com/yourusername/your-repo.git
cd your-repo
```

2. Install the project dependencies:

```bash
npm install
```

3. Once you've installed the project you can start the development server:

```bash
npm run dev

```

4. Access the application in your web browser at http://localhost:5173





