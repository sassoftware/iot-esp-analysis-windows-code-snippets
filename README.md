# ESP Analysis Windows Code Snippets

> The code snippets in this repository are designed to be executed with SAS Event Stream Processing 6.2 . For examples that you can execute with SAS Event Stream Processing 2020.1, refer to the SAS Event Stream Processing Studio Examples GitHub repository.


## Overview

This repository includes code snippets that you can execute for the Analysis windows of SAS Event Stream Processing (ESP). There is a directory for each example that contains all the files you need to execute the example. There is also a document for each code snippet to provide any instructions unique to the particular example.

The following sections list the examples and provide a description of each. You can click on the name of each example to go to the appropriate diretory containing the files.

### Calculate Window

Calculate windows create real time, running statistics that are based on established analytical techniques. They receive data events and publish newly transformed score data into output events.

| Example | Description |
| ------ | ------ |
| [analytics_changedetection](examples/calculate/analytics_changedetection) | This project is a basic demonstration of using the Change Detection	(ChangeDetection) algorithm. With change detection, a stream of measures is monitored and an alert is raised when values deviate from what is expected. |
| [analytics_cepstrum](examples/calculate/analytics_cepstrum) | This example is a basic demonstration of using the Cepstrum Transform (Cepstrum) algorithm. A cepstrum results from taking the inverse Fourier transform of the logarithm of the estimated spectrum of a signal. This application is often used in speech analysis, specifically with voice detection. |

### Train and Score Windows

Train windows receive data events and publish model events to Score windows. They use incoming data events to develop and adjust model parameters in real time. Score windows accept model events to make predictions for incoming data events. They generate scored data. You can use this score data to generate predictions based on the trained model. The following examples use Train and Score windows in the same model:

| Example | Description |
| ------ | ------ |
| [analytics_kmeans](examples/train_score/analytics_kmeans) | This project demonstrates the use of the learning algorithm for the online K-means clustering in ESP. It has has a single continuous query with a source window that receives the data to be scored, a train window that generates and periodically updates the k-means model, and lastly a score window that does the scoring. | 
| [analytics_dbscan](examples/train_score/analytics_dbscan) | This project demonstrates the use of the learning algorithm for the online DBSCAN clustering in ESP. It has a single continuous query with a source window that receives the data to be scored, a train window that generates and periodically updates the DBSCAN model, and lastly a score window that does the scoring. |


 
## Contributing

> We welcome your contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to submit contributions to this project. 

## License

> This project is licensed under the [Apache 2.0 License](LICENSE).

## Additional Resources

* [SAS Event Stream Processing 6.2 Product Documentation](https://go.documentation.sas.com/?cdcId=espcdc&cdcVersion=6.2&docsetId=espov&docsetTarget=home.htm&locale=en)
