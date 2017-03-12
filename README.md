# MIQP solver based on OSQP
The solver lives in the `miosqp` package. In order to run it you need to install the [OSQP Python interface](https://github.com/bstellato/osqp).

## Run example
In order to run the examples from to compare with GUROBI, after installing the python insterface, you need to install [mathprogbasepy](https://github.com/bstellato/mathprogbasepy). Examples can be found in the `examples` folder.

-   Random MIQPs
-   Power system example

Note that you need [pandas](http://pandas.pydata.org/) package for storing the results dataframe and [tqdm](https://github.com/noamraph/tqdm) package for the progress bar.


## Maximum number of iterations
For some problem instances, OSQP reaches the maximum number of iterations. In order to deal with them, they are dumped to different files in the `max_iter_examples` folder. In order to load them separately and solve them with OSQP, you can run the `run_maxiter_problem.py` file.
