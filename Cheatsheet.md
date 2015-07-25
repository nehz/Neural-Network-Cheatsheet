# Neural Network Cheatsheet

## Feedforward
### Activations
* Use `ReLU`. Try `tanh` but it is unlikely to perform better.
* Always use `tanh` in preference to `sigmoid`
(both similar, but `tanh` is zero centered, which is preferred )
* `ReLU`: greatly improves learning *rate*.
Very popular but has "dying unit" problem.
* `ReLU`: Be careful with learning rates to avoid dead units;
monitor how much of network is "dead"
* `ReLU`: Consider `Leaky ReLU` or `Maxout` if dead units are a problem.
* `Maxout`: Generalized form of `ReLU` and 'Leaky ReLU`, better,
but also doubles the amount of parameters per neuron


## RNN
### Layer units
* Use LSTM, GRU
* [MUT1-3][1] is also very promising

### Parameters
####LSTM
* Use bias of 1 on forget gate


## Sources
[1]: http://jmlr.org/proceedings/papers/v37/jozefowicz15.pdf
[2]: http://cs231n.github.io/
