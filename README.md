# Intelligent Document Organization 

The Intelligent Document Organization system is an AI-driven solution designed to optimize document management by automating the categorization and relocation of files within Google Drive. Using advanced tools like Pinecone and the Google Drive API, this system streamlines organizing large volumes of digital documents by analyzing content and recommending appropriate folders.  

### **Features**  
- **Automated File Categorization**: Classifies documents based on their content, offering folder suggestions.  
- **Google Drive Integration**: Directly uploads and organizes files within Google Drive.  
- **AI-Powered Folder Recommendations**: Utilizes content analysis to recommend suitable folders for each document.  
- **User-Friendly Interface**: Provides a seamless interface for file uploads and organization.  
- **Scalable and Efficient**: Handles high document volumes with impressive speed and accuracy.  

### **Project Workflow**  
1. **File Upload**: Users upload documents via a simple interface.  
2. **Content Analysis**: AI techniques analyze document content to determine its context.  
3. **Folder Suggestions**: Based on the analysis, the system recommends the most suitable folder.  
4. **File Organization**: Users can relocate the document to the suggested folder or leave it in its original location.  

### **Prerequisites**  
To run the project, ensure the following:  
- **Python 3.x installed.**  
- **Google Drive API credentials with service account access.** 
- **Optional: Google Colab or a local Python environment for execution.**

### **Setup Instructions for Intelligent Document Organization**  

1. **Clone the Repository**
2. **Install Dependencies**:  
   Install the necessary Python libraries required for running the Intelligent Document Organization system. You can install them using the following command:  
   ```bash  
   pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib pinecone-client  
   ```
3. **Obtain Google Drive API Credentials**:  
   To interact with Google Drive, you will need to enable the Google Drive API and create OAuth 2.0 credentials:  
   - Go to the [Google Developers Console](https://console.developers.google.com/).  
   - Create a new project.  
   - Enable the **Google Drive API** for that project.  
   - Generate OAuth 2.0 credentials and download the credentials JSON file.  

   Save the credentials file as `credentials.json` in the project directory.

4. **Set Up Pinecone API**:  
   To enable AI-powered document organization, you need a Pinecone account for indexing document content.  
   - Create an account at [Pinecone.io](https://www.pinecone.io/).  
   - Get your Pinecone API key from your dashboard.  
   - Create an index and store the key securely in the project.

5. **Configure API Keys and Credentials**:  
   - Update the `config.py` file in the repository with your **Google API credentials** (the path to `credentials.json`) and **Pinecone API key**.  
   - If using Google Colab, upload the `credentials.json` file and configure the environment as needed.

6. **Run the Project**:  
   After completing the setup, run the Python script to start the intelligent document organization process:  
   - In Google Colab, execute the cells in the notebook.  
   - For local execution, run the following command:  
   ```bash  
   python organize_documents.py  
   ```
7. **Upload and Organize Documents**:  
   Once the system is running, you can begin uploading documents to Google Drive. The system will automatically analyze their content and suggest suitable folders for organizing them.

8. **Troubleshooting**:  
   - Ensure the `credentials.json` file is correctly configured and accessible in your working directory.  
   - Verify that the Pinecone API key is valid and correctly entered.  
   - Make sure the Google Drive API is properly authenticated before running the code.

### **Skills Demonstrated**  
1. **Artificial Intelligence**: Leveraged AI tools like Pinecone for intelligent content analysis and recommendation generation.  
2. **API Integration**: Implemented the Google Drive API for seamless document upload and organization.  
3. **Machine Learning**: Applied techniques to automate document categorization and folder recommendations.  
4. **Data Handling**: Processed and analyzed large volumes of documents with high accuracy.   
5. **Content-Based Recommendation Systems**: Developed algorithms to analyze document content for intelligent folder suggestions.    
6. **System Scalability**: Designed a solution capable of handling large datasets while maintaining performance.  

### **Project outcome**  
The system demonstrates high accuracy in categorizing documents and recommending folders, significantly simplifying document management. Users have praised its intuitive design, ease of use, and efficiency in handling large-scale document organization tasks.
