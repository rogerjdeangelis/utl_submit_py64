# utl_submit_py64
Interface to Python 2.7 from SAS/WPS

    ```  Python: Projection of the intersection of two paraboliods onto the xy plane  ```
    ```    ```
    ```  We will show that the projection of the intersection of two paraboliods is a circle  ```
    ```  in the xy plane. This is a very simple example of a general technique.  ```
    ```    ```
    ```       WORKING CODE  ```
    ```       ============  ```
    ```    ```
    ```          x, y = sym.symbols('x y', real=True);  ```
    ```    ```
    ```          z1 = 2*x**2 + 3*y**2     * two surfaces;  ```
    ```          z2 = 5 - 3*x**2 - 2*y**2  ```
    ```    ```
    ```          sol = sym.solve(z1-z2, y);  ```
    ```          print(sol);  ```
    ```    ```
    ```          The solution can be manually derived algebraically  ```
    ```    ```
    ```              2*x**2 + 3*y**2 = 5 - 3*x**2 - 2*y**2  ```
    ```              5 = 5*x**2 + 5*y**2  ```
    ```              1 = x**2 + y**2    (unit circle)  ```
    ```    ```
    ```    us a period in position 1 for indented python code see my SAS-L posts```
    ```  see  ```
    ```  https://goo.gl/HVcsMf  ```
    ```  https://stackoverflow.com/questions/45130525/  ```
    ```  find-the-equation-y-yx-from-the-intersection-of-two-surfaces-z-zx-y  ```
    ```    ```
    ```  also  ```
    ```  http://www.math.wvu.edu/~hjlai/Teaching/Tip-Pdf/Tip3-18.pdf  ```
    ```    ```
    ```  Ales profile  ```
    ```  https://stackoverflow.com/users/6655984/alex  ```
    ```    ```
    ```    ```
    ```    ```
    ```  HAVE  ```
    ```  ====  ```
    ```    ```
    ```     z1 = 2*x**2 + 3*y**2  ```
    ```     z2 = 5 - 3*x**2 - 2*y**2  ```
    ```    ```
    ```    This depiction does not correspond the the example below but  ```
    ```    may help in understand the problem  ```
    ```    ```
    ```    ```
    ```                    +-------------+-------------+-----------+  ```
    ```                   /             /             /   x       /|  ```
    ```                  /             /             /  x        / |  ```
    ```                 /             /             / x         /  |  ```
    ```                /             /             /x          /   |  ```
    ```               /             /             x           /    |  ```
    ```              /             /            x/           /     + Y  ```
    ```             /-------------/-----------x-*-----------/     /  ```
    ```            /             /          x */           /     /  ```
    ```           /             /         x | /           /     /  ```
    ```          /             /        x | */           /     /  ```
    ```         /             /      x  | | /           /     /  ```
    ```        /             /    x  |  | */           /     /  ```
    ```       /      x x x  x  ^  |  |  * /           /     /  ```
    ```      +-------------/-------------+--------- +/     /  ```
    ```      |    /  | | |/ |  |  |  |  /           |     /  ```
    ```      |   /   | | |  |  |  |  * /            |    /  ```
    ```      |  /    | |/|  |  |  |   /             |   /  ```
    ```      | /     | | |  |  |  *  /              |  /  ```
    ```      |/      */* *  *  *    /               | /  ```
    ```    Z +-------+-------------+----------------+/  ```
    ```    ```
    ```  *                    _  ```
    ```  __      ____ _ _ __ | |_  ```
    ```  \ \ /\ / / _` | '_ \| __|  ```
    ```   \ V  V / (_| | | | | |_  ```
    ```    \_/\_/ \__,_|_| |_|\__|  ```
    ```  ;  ```
    ```    ```
    ```        1 = y**2 + x**2  ```
    ```    ```
    ```    ```
    ```  %utl_submit_py64("  ```
    ```  import sympy as sym;  ```
    ```  x, y = sym.symbols('x y', real=True);  ```
    ```  z1 = 2*x**2 + 3*y**2;  ```
    ```  z2 = 5 - 3*x**2 - 2*y**2;  ```
    ```  sol = sym.solve(z1-z2, y);  ```
    ```  print(sol);  ```
    ```  ");  ```
    ```    ```
    ```    ```
    ```  *          _       _   _  ```
    ```   ___  ___ | |_   _| |_(_) ___  _ __  ```
    ```  / __|/ _ \| | | | | __| |/ _ \| '_ \  ```
    ```  \__ \ (_) | | |_| | |_| | (_) | | | |  ```
    ```  |___/\___/|_|\__,_|\__|_|\___/|_| |_|  ```
    ```    ```
    ```  ;  ```
    ```    ```
    ```  Quadratics have two solutions  ```
    ```  (in this case they both give the same real solution).  ```
    ```    ```
    ```  [-(-x**2 + 1)**(1/2), (-x**2 + 1)**(1/2)]  ```
    ```    ```
    ```    y= -(-x**2 + 1)**(1/2);  ```
    ```    y**2= -x**2 + 1  ```
    ```    1 = y**2 + x**2  ```
    ```    ```
    ```    ```
