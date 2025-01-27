Important Links:

GCP Project ID: lofty-fragment-448721-a0 ([link](https://console.cloud.google.com/home/dashboard?hl=en&inv=1&invt=Abn5dw&project=lofty-fragment-448721-a0)) 

Service name: [Cloud Speech-to-Text API](https://console.cloud.google.com/apis/api/speech.googleapis.com/overview?hl=en&inv=1&invt=Abn5dw&project=lofty-fragment-448721-a0), [Text-to-Speech API](https://console.cloud.google.com/apis/api/texttospeech.googleapis.com/overview?hl=en&inv=1&invt=Abn5dw&project=lofty-fragment-448721-a0)

App URL: https://assignment1-426819123137.us-central1.run.app

Introduction:

The project is a web-based application that uses Google Cloud's Speech-to-Text and Text-to-Speech services to handle audio and text processing. The main objective of the project is to provide a platform where a user can convert text into speech and speech into text. The user will be able to record audio or type some text, which will be uploaded and converted to text or speech based on selection using google APIs.

Key Features:

1.  Audio file upload and converted to text using Google Speech to Text API

2.  Text file upload and converted to audio using Google Text to Speech API

3.  Storage, organisation and retrieval of files

Architecture:

The application was built using Flask, which is a lightweight web application. The following are the main components:

1.  Flask Based Web Application:

-   Acts as the central control for user interactions and back-end processing.

-   Manages routes for uploading files, converting formats, and retrieving data.

2.  Google Cloud APIs:

-   Speech-to-Text API: Transcribes audio files into text.

-   Text-to-Speech API: Synthesizes audio files from text inputs.

3.  Storage:

-   Local File Storage: All uploaded and generated files are stored in a directory.

4.  User Interface:

-   Interact with the application through a web based user interface to upload files and view results.

Functionality of components:

-   Flask Framework: Providing a lightweight framework for the architecture, routing and user interface.

-   Google Cloud APIs: Used to convert the contents provided by the user and produce the required results.

-   Local Storage: Ensures the storage and the easy access of the contents.

-   User Interface: It provides a medium for the user to interact with the API's and the storage to carry out the required task.

Implementation:

The project's implementation involved setting up Flask, integrating Google Cloud APIs, and building a structured workflow for audio and text processing.

Dependencies:

1.  Flask: For building the web application.

2.  google-cloud-speech: For accessing Google's Speech-to-Text API.

3.  google-cloud-texttospeech: For accessing Google's Text-to-Speech API.

4.  datetime: For generating timestamps used in file naming.

5.  os: For file system interactions.


Workflow:

1.  Audio Upload and Transcription:

-   Users upload .wav files.

-   The server processes the file, calls the Speech-to-Text API, and saves the transcription in .txt format.

2.  Text Input and Audio Generation:

-   Users input text through a form.

-   The server calls the Text-to-Speech API to generate a .wav file from the text.

3.  File Management:

-   Uploaded and generated files are time stamped for easy identification.

-   Files can be retrieved through dedicated routes.

Pros and Cons: 

### Pros:

1.  Ease of Use: The application has a simple and intuitive interface.

2.  Scalable APIs: By leveraging Google Cloud, the solution ensures high accuracy and scalability for audio-text conversion.

### Cons:

1.  Scalability Issues: Local file storage may become a bottleneck as the number of users increases.

2.  Concurrency: The app lacks features like load balancing or a queue system to handle multiple users simultaneously.


Application instructions: 

1.  Uploading Audio Files:

-   Navigate to the homepage.

-   Click on Start to start recording the audio and stop to stop the audio recording.

-   Wait for processing and view the txt file

2.  Uploading Text for Speech Generation:

-   Navigate to the homepage.

-   Enter text into the form and click upload.

-   Play the generated .wav file.

3.  Viewing Files:

-   All uploaded and generated files are listed on the homepage.

-   Click on any file to view it.

Screenshots:

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeEdCJMEFs9JlfGzGZQcSGll0bU9bb97yZvFozYoWkiKWOO51xs23RepL70rJi6zLq58ptenp-hen0PREyoDTpiR7sTqui4WWEp91G7t4442VzppbfZcNMXCgkj_NzgAFliHr5dCw?key=ljfbg-IdJDXERtO0jyVmNkEK)

Lessons Learned:
----------------

-   Gained experience in deploying Flask based apps on Google Cloud Platform.

-   Learned the implementation of Google API's.

-   Improved knowledge of file handling and naming conventions.
