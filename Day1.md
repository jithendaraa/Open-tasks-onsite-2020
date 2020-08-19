## Day 1

### Tasks (Domain: ML)

#### Task 1

1. **Part 1:** Create your own synthetic dataset from a nonlinear univariate function <img src="https://render.githubusercontent.com/render/math?math=y = f(x)"> and fit a regression model to this using a neural network.

    ##### Steps

    1. Decide on a nonlinear univariate function <img src="https://render.githubusercontent.com/render/math?math=y = f(x) \space"> like
       1. <img src="https://render.githubusercontent.com/render/math?math=y= sin(9 sin^{3}(x %2B 1.8) - 1) \space"> where <img src="https://render.githubusercontent.com/render/math?math=x \in [1,e] - 1.8"> or 
       2. <img src="https://render.githubusercontent.com/render/math?math=y= tanh(10x %2B 4) - tanh(10x %2B 3) %2B tanh(10x - 4) - tanh(10x-3) \space"> where <img src="https://render.githubusercontent.com/render/math?math=x \in [-1,1]">

    2. Sample 'n' datapoints <img src="https://render.githubusercontent.com/render/math?math=x"> from a uniform distribution within the given range of <img src="https://render.githubusercontent.com/render/math?math=x">. For every datapoint, get the corresponding  as <img src="https://render.githubusercontent.com/render/math?math=y=f(x) %2B \epsilon, \epsilon ~ N(0,1)">
    3. Plot the true function <img src="https://render.githubusercontent.com/render/math?math=y = f(x) \space"> and a scatter plot of datapoints from your synthetic dataset to get an idea of the noise introduced by ε. If you feel there's too much noise, you are free to reduce the std. dev. of the normal distribution that ε came from (eg. reducing it from 1 to 0.5 might help)
    4. Build a neural network (but don't make it too deep; it might overfit!) to fit your synthetic dataset. You are free to use any deep learning framework like TensorFlow or PyTorch.

2. **Part 2:** Same as "Part 1" above but don't use a DL framework for step 4; use NumPy!
   
3. **Part 3** Same as "Part 1" above but this time, do it for a multivariate function in N variables <img src="https://render.githubusercontent.com/render/math?math=y = f(x1, x2, ... xN) \space">

4. **Part 4** Same as "Part 3" above but don't use a DL framework for step 4; use NumPy!

### Tasks (Domain: Game Dev)

1. Make a 3D game similar to Subway surfers, to clarify, the player can - Jump, Move left or right, and bend under obstacles of various shapes. The task of the player is to reach as far as he can without hitting the obstacle and collect as many gold coins on the way as possible (the game can be very basic in design)

#### Features

1. The player be able to jump, or bend down or move left or right in order to avoid obstacles (obstacles of different shapes).

2. There must be a scoreboard at the end of the game, which shows the top 5 scores on the same system.

Feel free to be creative and add any new features you can come up with.
