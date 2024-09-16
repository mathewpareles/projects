This notebook analyzes GPT's ability to solve LEGO problems (https://arxiv.org/pdf/2206.04301.pdf)

See points 3) and 4) below for results

1) In 'data_iterate.ipynb':

We iterate:

	Generate a LEGO system of equations (SOE) and a hint (HINT) towards solving it

	Define the string concatenation PROMPT = SOE + HINT

	Write the result to the './data' folder

2) In 'analysis.ipynb':

	We pass the various prompts into './data' to GPT-3

	We analyze the accuracy (results are graphs)

3) Results:

3.* folders:

	equals signs are padded with spaces; naming convention is (pad SOE) / (pad hint)

4.* folders:

	variables are named numerically "a13 = -b20"

	results: GPT-3 successfully solves SOEs with many variables


5.* folders:

	variables have spaces/commas between tokens. For example: "a 1 0 = -b 7 2" or "a,1,0 = -b,7,2"

	results: successful in small-length regime

6.* folders:

	variables are words "the lazy = - dog"

	results: successful


4) Future work

	What is the underlying attention pattern? Does it generalize to other reasoning tasks?
	

