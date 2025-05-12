# spinning-donuts
spinning donut, revamped for github pages

## How to Run

### Prerequisites
To run this project, you need:
- A C compiler (such as `gcc`)
- A Unix-based system (Linux or macOS) to use the `usleep` function for managing the animation speed

### Steps:
1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/your-username/donut-animation.git
    ```

2. Navigate to the project folder:
    ```bash
    cd donut-animation
    ```

3. Compile the C code:
    ```bash
    gcc donut.c -o donut
    ```

4. Run the compiled executable:
    ```bash
    ./donut
    ```

You should see the donut animation spinning in your terminal window.

### Customizing Speed:
To adjust the speed of the donut's rotation, you can modify the `usleep` function in the code. The current setting is `usleep(30000);`, which controls the speed. A higher value will slow down the animation, and a lower value will speed it up.

## Project Structure

- `donut.c`: The main C file that generates the spinning donut animation.
- `README.md`: This file, containing project details and setup instructions.

## About the Animation

The donut is rendered using a combination of trigonometric functions (`sin`, `cos`) to calculate its 3D shape. The ASCII characters are updated frame by frame, creating the illusion of a rotating donut.

### How It Works:
- The code calculates the positions of points on a 3D donut using spherical coordinates.
- The points are then mapped to a 2D screen and updated to give the appearance of rotation.
- The ASCII characters (`.,-~#@$*)`) are used to represent the donut at different depths.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to [John D. Cook](https://www.johndcook.com/) for the inspiration for the mathematical formulas used in this animation.
- Special thanks to open-source communities for providing valuable resources and tools.
