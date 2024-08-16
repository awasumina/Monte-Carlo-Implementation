# Monte Carlo Method to Estimate π

This project uses the Monte Carlo method to estimate the value of π (pi) by simulating random points within a quarter circle. The estimation is based on the ratio of points that fall inside the quarter circle versus those that fall outside.

The Monte Carlo method involves generating random points in a given area and determining the ratio of points that fall inside a defined shape (in this case, a quarter circle). This ratio is then used to estimate π.


## Code Explanation

1. **Generate Random Points**
   - Random points are generated within a square of side length equal to the radius of the quarter circle.

2. **Determine Points Inside the Quarter Circle**
   - Points that fall inside the quarter circle are determined using the equation \( x^2 + y^2 \leq r^2 \).

3. **Estimate the Area**
   - The area of the quarter circle is estimated based on the ratio of points inside the circle.

4. **Estimate π**
   - Using the estimated area of the quarter circle, π is estimated by multiplying the area by 4 and normalizing by the area of the full circle.

5. **Plotting**
   - A plot is generated showing the quarter circle, points inside the circle (green), and points outside the circle (red).


## Results

- **Estimated π**: The estimated value of π based on the Monte Carlo simulation.
- **Analytical π**: The actual value of π as provided by NumPy.
- **Error**: The absolute difference between the estimated and actual values of π.
- **Error %**: The percentage error of the estimation.


##  Output

Estimated π=3.228
Analytical π=3.141592653589793
Error = 0.08640734641020709
Error % = 2.75%


## Plot

The plot generated by the script displays:

- The quarter circle in blue.
- Points inside the quarter circle in green.
- Points outside the quarter circle in red.



## Conclusion

The Monte Carlo method provides an estimate of π that is reasonably close to the analytical value. Despite the inherent randomness of the method, the estimated value of π is fairly accurate with a small error margin of 2.75%. The accuracy of the estimate can be improved by increasing the number of random points, demonstrating the method's potential for approximating complex mathematical constants through statistical simulation. 
