# Overview

Create a plain text histogram at the command line. 

This is a Python 3 port of `histogram.py` from [data_hacks](https://github.com/bitly/data_hacks/blob/master/data_hacks/histogram.py)

# Install

    $ curl https://raw.githubusercontent.com/clarkgrubb/histogram/master/histogram > /usr/local/bin/histogram
	$ chmod +x /usr/local/bin/histogram

# Use

	$ awk '{print length($0)}' /etc/passwd | histogram
	# NumSamples = 103; Min = 1.00; Max = 96.00
	# Mean = 61.067961; Variance = 296.296352; SD = 17.213261; Median 63.000000
	# each ∎ represents a count of 1
	    1.0000 -    10.5000 [     4]: ∎∎∎∎
	   10.5000 -    20.0000 [     3]: ∎∎∎
	   20.0000 -    29.5000 [     0]: 
	   29.5000 -    39.0000 [     0]: 
	   39.0000 -    48.5000 [     0]: 
	   48.5000 -    58.0000 [    26]: ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
	   58.0000 -    67.5000 [    32]: ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
	   67.5000 -    77.0000 [    29]: ∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎∎
	   77.0000 -    86.5000 [     7]: ∎∎∎∎∎∎∎
	   86.5000 -    96.0000 [     2]: ∎∎
