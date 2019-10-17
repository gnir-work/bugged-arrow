## Bugged arrow
In this repo you will find a bugged version of arrow.
In general this repo was created as an exercise in debugging a big code base.
The code itself wasn't written by me, you can check the original repo [here](https://github.com/crsmithdev/arrow)

## The bugs
* In `arrow/parser.py` the function `_parse_token` used to recieve the paramters `parts` and mutate it, now it mutates a default parameter and therefor each call to the function the parts from the previous call are saved.
* In `arrow/parser.py`, line `41`, the `TWO_DIGITS` regex actually searched for three digits.
* In `arrow/api.py` typo in line `32`, `_factory.utnow` -> `_factory.utcnow`.   
