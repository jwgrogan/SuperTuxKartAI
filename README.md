# rocketleagueAI-dl-su20
Term project for Deep Learning


### To train this ish:

1. Unzip `data.zip` into the project directory
2. Increment the `--run` env variable found on line 116 of `agent/train.py`
2. Run: `python -m agent.train <add env variables here OR more on that below>`

**Note** Refer to `agent/train` to see the hyperparameters that you can tweak...also feel free to "hard-code" those parameters in the bottom of the file as well. 


### To play da game with 2 Players:

1. Run `python -m tournament.play agent agent -s gameplay/`

**Note** After this finishes running, there should be a `.mp4` file in `gameplay` for each of the 2 players.


### If you want to generate new data.

TLDR:

1. Run 
```
python -m tournament.gen_train_data random_agent random_agent random_agent random_agent -s data\train -f 1600
```

**Note** There's a lot of different ways to do this but couple of tips to follow.
- make sure that whatever value in `-f` multiplied by the number of "random_agent"s is a multiple of 64, 128, 256 (our typical batch sizes) 

Hit Lewai up too cuz there's a couple of commands and it could get messy/complicated.