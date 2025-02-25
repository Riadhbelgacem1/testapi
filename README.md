To test your Flask API with Postman, follow these steps:

Open Postman: Launch the Postman application on your computer.

Create a New Request:

Click on the “New” button or use the “+” tab to open a new request.
Set the request method to POST.
Set the Request URL:

Enter the URL of your Flask API endpoint. For local testing, it would be http://127.0.0.1:5000/predict.
Add Form Data:

Click on the “Body” tab.
Select the “form-data” option.
In the “KEY” field, enter file (this should match the name used in request.files['file'] in your predict route).
Set the type of the value to “File” (you can do this by clicking on the dropdown next to the “Text” type and selecting “File”).
Click on the “Choose Files” button that appears and select the .tif file you want to upload.
Send the Request:

Click the “Send” button.
You should see the response from your Flask API in the response pane below, which should include the message and the path to the saved prediction file.
Verify the Response:

Ensure the message "Prediction done" appears, and the output_path points to the correct path where the prediction file is saved.
If you encounter any issues, make sure your Flask server is running and accessible at the specified address.
