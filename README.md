## How to code the Koch Snowflake

- Recursive Step: At each recursive step, the line segment is split into three equal parts. Then, a new point is added above the middle part to form an equilateral triangle, creating the bump that defines the snowflake shape. The middle third is replaced with the two new sides of the triangle, turning one segment into four smaller ones.
- Base Case:  The recursion stops when the line segment becomes very short, typically just a few pixels. At this point, the segment is drawn as a straight line, preventing endless calculations and ensuring the fractal has the desired level of detail.
- Translate and Rotate: The translate function moves the starting point of a line to make calculations easier, and rotate turns the line to line up horizontally. After using these, pop() resets everything back to normal for the next line.
