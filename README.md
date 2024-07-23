PostKeeper App
The PostKeeper App is a simple image gallery application that allows users to save their favorite images with a single click. Users can view all their saved images by clicking the 'Saved Posts' button located in the navbar. Additionally, users can unsave images and reset the entire saved list.

Features
Save Images: Users can save images by clicking the save icon on each image.
View Saved Images: Users can view their saved images by clicking the 'Saved Posts' button in the navbar.
Unsave Images: Users can unsave images by clicking the unsave icon on saved images.
Reset Saved List: Users can reset the entire saved list by clicking the 'Reset' button.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/postkeeper-app.git
cd postkeeper-app
Install the dependencies:

bash
Copy code
npm install
Run the application:

bash
Copy code
npm start
The application will run on http://localhost:3000.

File Structure
plaintext
Copy code
.
├── src
│   ├── App.js
│   ├── List.js
│   ├── Navbar.js
│   ├── postContext.js
│   ├── data.js
│   └── styles.css
├── public
│   ├── index.html
│   └── ...
├── package.json
└── README.md
Usage
App Component
The App component is the root component of the application. It includes the PostContextProvider which provides the context to the Navbar and List components.

Navbar Component
The Navbar component displays the number of saved posts and a list of saved posts when the 'Saved Posts' button is clicked. It also includes a Reset button to clear all saved posts.

List Component
The List component displays a list of posts. Each post can be saved by clicking the save icon, or unsaved by clicking the unsave icon.

postContext.js
The postContext.js file contains the context logic for managing saved posts. It includes functions for saving, unsaving, and resetting posts. The usePostsValue custom hook is used to access the context in other components.

data.js
The data.js file contains an array of post objects, each with an id, text, and img URL.

styles.css
The styles.css file contains the styles for the application.

Contributing
Contributions are welcome! Please open an issue or submit a pull request.
