# YouTube Video Manager (CLI)

This project is a Command-Line Interface (CLI) application built with Python and the `pymongo` driver. It acts as a YouTube Video Manager, allowing users to efficiently track video titles and durations. The application connects to a MongoDB database to perform core CRUD (Create, Read, Update, Delete) operations, demonstrating practical experience with NoSQL databases and basic Python scripting.

## 🚀 Features

* **List all videos:** View the unique IDs, names, and durations of all saved videos in the database.
* **Add a video:** Store a new video with its name and timestamp/duration.
* **Update a video:** Modify the details of an existing video using its unique MongoDB `ObjectId`.
* **Delete a video:** Remove a video completely from the database.

## 🛠️ Tech Stack

* **Language:** Python 3
* **Database:** MongoDB (via MongoDB Atlas)
* **Libraries:** `pymongo`, `bson`

## 📋 Prerequisites

Before running this project, ensure you have the following installed:
* [Python 3.x](https://www.python.org/downloads/)
* A [MongoDB Atlas Account](https://www.mongodb.com/cloud/atlas) or a local MongoDB server.

## ⚙️ Installation

1. **Clone the repository:**
   bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
   cd your-repo-name

2. Install the required dependencies:
   This project requires the pymongo driver to interact with the database.

   
   pip install pymongo

3. Configure your Database:

   Open the main.py script.

   Locate the MongoClient connection string and replace it with your own MongoDB URI.

   Note: For security reasons, it is highly recommended to use environment variables (e.g., python-dotenv) in production rather than hardcoding credentials.

4.💻 Usage
  Run the script from your terminal:

  Bash
  python main.py

🔮 Future Enhancements
Implement python-dotenv to securely hide the MongoDB URI string and credentials.

Add try...except blocks for graceful error handling (e.g., handling invalid MongoDB ObjectIds).

Add a search feature to filter videos by name.
