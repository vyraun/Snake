# Snake
Toy example of a deep reinforcement model playing the game of Snake. It's a follow up to a similar model that has learned to catch fruit: https://github.com/bitwise-ben/Fruit.

<img src="images/snake.gif" />

After a few (code) iterations, the model has learned to get to fruit in fewer steps, and stay alive longer.

I'm not sure how much more training is required for the model to become better. The grid size is relatively small (10 x 10), and thus games quickly become difficult as the snake gets longer.

By now, training takes a considerable amount of time, and probably another reinforcement learning algorithm (e.g., A3C) is necessary to keep training time within reasonable bounds.

#Error

Traceback (most recent call last):
  File "snake.py", line 167, in <module>
    loss += model.train_on_batch(np.array(inputs), np.array(targets))[0]
IndexError: too many indices for array

