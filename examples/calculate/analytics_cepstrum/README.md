# analytics_cepstrum Instructions

This example is a basic demonstration of using the Cepstrum Transform (Cepstrum) algorithm. A cepstrum results from taking the inverse Fourier transform of the logarithm of the estimated spectrum of a signal. This application is often used in speech analysis, specifically with voice detection.

Use the following steps to execute the analytics_cepstrum code snippet:

1.  Create a directory on the ESP server for the example.

2.  Upload the `input.csv` file to the server directory you just created.

3.  Upload the `model.xml` file to SAS ESP Studio. Refer to the [Uploading a Model to ESP Studio](../../../docs/Uploading_a_Model_to_ESP_Studio.pdf) document for instructions.
  
4.  Double-click the project named `project_01` to open it.

5.  Edit the Input Data Connector for the `w_source` window to include the full path to the `input.csv` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

6.  Edit the Subscriber Connector for the `w_calculate` window to include the full path to the `result.out` file you uploaded. Refer to the [Editing Connectors](../../../docs/Connectors.pdf) document for instructions.

7.  Save your changes and test your model. Refer to the [Testing Models](../../../docs/Testing_Models.pdf) document for instrcutions.

8.  Execute the model on the ESP Server and Subscribe to the `w_calculate` window using ESP Streamviewer. Refer to the [Executing a Model and Viewing the Output](../../../docs/Executing_a_Model_and_Viewing_the_Output.pdf) document for instructions.


