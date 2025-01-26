MediCare
MediCare is a React-based web application designed to help users locate medical centers across the country by selecting their state and city. Users can book appointments, explore specializations, and view their past bookings. The application ensures ease of access to healthcare facilities with an intuitive and user-friendly interface.

Features
1. Landing Page
Navigation Bar: Access various platform sections such as Find Doctors, Hospitals, and Medicines.
State and City Search: Dropdown menus fetch available states and cities from an API, enabling users to view medical centers in their selected area.
Hero Section: A visually appealing introduction with state and city selection.
Specializations Section: Displays available medical specialties for users to explore.
Blogs and Insights: Provides blogs and statistics on user engagement.
Download App: Dedicated section to promote mobile app downloads.
Footer: Useful links and contact details.
Screenshots:
Landing Page




2. Slot Booking
Medical Center Selection: Choose from a list of hospitals or centers in the selected city.
Appointment Booking:
Calendar interface to select an appointment date (from today up to one week in advance).
Available time slots for the chosen day.
Booking Confirmation: Receive a confirmation via email.
Screenshots:
Available Hospitals

Date and Time Selection

Booking Confirmation

3. Past Bookings
Personalized Dashboard: Users can view all their past bookings.
Details: Includes medical center name, appointment date, and time.
Screenshot:
Past Bookings

API Endpoints
1. Get All States
Fetch a list of all available states.

http
Copy
Edit
GET https://meddata-backend.onrender.com/states
2. Get Cities in a State
Fetch cities within a selected state.

http
Copy
Edit
GET https://meddata-backend.onrender.com/cities/:state
Example:
GET https://meddata-backend.onrender.com/cities/Karnataka

3. Get Medical Centers
Fetch all medical centers based on state and city.

http
Copy
Edit
GET https://meddata-backend.onrender.com/data?state=<state-name>&city=<city-name>
Example:
GET https://meddata-backend.onrender.com/data?state=Karnataka&city=Bangalore

Installation and Setup
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/PK1812KHARE/MediCare.git
cd MediCare
2. Install Dependencies
bash
Copy
Edit
npm install
3. Start the Development Server
bash
Copy
Edit
npm start
The application will run on http://localhost:3000.

Technologies Used
Frontend: React.js
Styling: CSS, Bootstrap
APIs: Custom backend hosted on Render
Tools: Git, npm
Contributing
Contributions are welcome! If you’d like to contribute:

Fork the repository.
Create a new branch:
bash
Copy
Edit
git checkout -b feature-name
Commit your changes:
bash
Copy
Edit
git commit -m "Description of changes"
Push to your branch:
bash
Copy
Edit
git push origin feature-name
Submit a pull request.
