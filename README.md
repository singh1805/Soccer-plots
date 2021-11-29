# Soccer-plots
To plot the probability of a goal based on its x and y coordinates for sample data from 3 major football leagues. (A very basic design using polyfit)

Problem Statement- Taking raw data for player shot locations and probability of the shot being a goal (xG), the program should:
1. Map the xG with respect to x-coordinate of shot for three sets of data from three major soccer leagues and create a polynomial regression curve to fit the data.
2. Map the xG with respect to y-coordinate of shot for three sets of data from three major soccer leagues and create a polynomial regression curve to fit the data.
3. Use the equation of the polynomial regression curves to predict xG (or likelihood of goal) for a user input x-coordinate or y-coordinate of shot.
4. Draw an accurate scale model of the football pitch and plot shot locations and xG of each shot represented by circles (size representative of xG) and use it to draw conclusions about the data.

Solution to the Problem- The problem was divided into steps, as shown below:
1. Import pickle package to read pickle files obtained from Github who has obtained the same from statsbomb.com
2. Obtain user input- which league's data does the user want to see?
3. Based on user input- choose the file from which data will be extracted and extract all data as variable shot_data
4. Then extract x coordinate, y coordinate and xG of shot (probability of goal) from the shot_data.
5. Scale the x coordinate and y coordinate of shot based on the standard football pitch size= 130 by 90 units
6. Create a polyfit model for fitting xG curve based on x coordinates (separately) and y coordinates (separately).
7. Create a scatterplot for xG and x coordinates (separately and y coordinates (separately), and plot the curves on them separately.
8. Create a football pitch using matplotlib and the exact dimensions of the pitch on which we want to plot the data- and plot x coordinates, y coordinates and xG of shot data on the pitch.
9. Take user input for x- or y- coordinates (within the range of data) and feed it to the xG model to get predictions of xG.
