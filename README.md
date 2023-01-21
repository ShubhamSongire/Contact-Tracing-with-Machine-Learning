# Contact-Tracing-with-Machine-Learning
This is a contact tracing program using machine learning by using this method government or local agencies can easily track people in situations like COVID-19 or security purpose about how many peoples are came in contact with specific person. Using machine learning clustering method I have made this code which helps to contact tracing.

# Getting Started
To use this code, you will need to have Python and the following libraries installed:

- numpy
- pandas
- seaborn
- matplotlib
- datetime
- sklearn

You will also need to have a JSON file called "livedata.json" containing the location data of people to be used as input for the code.

Code Structure
The code starts by importing necessary libraries and setting up the environment for visualization. It then reads in the "livedata.json" file and stores it in a pandas DataFrame called "df". The code then checks for any null values in the data and plots a graph using the latitude and longitude values, with each point colored according to the "id" of the person. The DBSCAN algorithm is then applied to find people who have come in contact with each other based on their location data. A function called "get_infected_name()" is defined which takes an input of a name and returns a list of people who came in contact with that person within 6 feet. In the last line of the code, the function is called with the input name "Bob" and returns "Judy had come in contact with the patient."

The output graph is a scatter plot of all the peoples latitude and longitude with their id on the graph and the output of the function is the name of people who came in contact with the patient.

Conclusion
This code can be useful for government or local agencies to track people in situations like COVID-19 or security purpose. The code can be easily modified to use other location data, or to change the parameters of the DBSCAN algorithm to better suit the specific use case. It can help to know about the people who came in contact with the specific person which will help in contact tracing.<br> 
### This is an output dashboard where the machine learning algorithm tracks people by creating clusters based on the radius specified.
<div align="center">
    <a href="./">
        <img src="https://user-images.githubusercontent.com/68246393/144760224-57cd18b6-701a-4ab4-98a6-5db1f5f542b0.png" width="59%"/>
    </a>
</div> <br>

<div align="center">
    <a href="./">
        <img src="https://user-images.githubusercontent.com/68246393/213873513-d87731aa-e75e-4cb3-9889-54ef4b968e25.png" width="59%"/>
    </a>
</div> <br>
### In the above output, we can see that there are only 2 people in this cluster. When we input "Bob" as the patient, the program returns "Judy" as an infected person.
