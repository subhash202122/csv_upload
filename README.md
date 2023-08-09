# CSV Upload to MongoDB Project

This project is a simple web application that allows you to upload a CSV file containing personal data (FirstName, LastName, and Age) and store it in a MongoDB database.

## Setup Instructions

1. **Clone the repository:**


   git clone https://github.com/your-username/csv-upload-mongodb.git
   cd csv-upload-mongodb
  

2. **Install Dependencies:**

   Ensure you have Node.js and npm (Node Package Manager) installed on your system. Then, install the project's dependencies:


   npm install


3. **Database Configuration:**

   Make sure you have a MongoDB server running locally or provide the appropriate MongoDB connection URL in the `index.js` file:


   mongoose.connect('mongodb://localhost:27017/csv_upload', {
     useNewUrlParser: true,
     useUnifiedTopology: true
   })
 

4. **Run the Application:**

   Start the Node.js server to run the application:

 
   node index.js


5. **Access the Application:**

   Open your web browser and navigate to `http://localhost:3000` to access the application. You'll see a form where you can upload a CSV file containing personal data.

6. **Upload a CSV File:**

   Choose a CSV file (format: FirstName, LastName, Age) and click the "Submit" button. The data will be parsed from the CSV file and stored in the MongoDB database.

## Dependencies

- Express.js
- Mongoose
- Multer
- csvtojson
