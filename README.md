# CoffeaJERC
Jet energy resolution and corrections with NANAOD and columnar analysis based on Coffea. 

## Set up a coffea-enabled environment at FNAL

Log into `cmslpc`: 

```
ssh -L localhost:8888:localhost:8888  <username>@cmslpc-sl7.fnal.gov
```

Get a voms ticket: 

```
voms proxy init -voms cms
```

Go to your working directory.  If this is your first time using this/you don't have a coffea environment with lpcjobqueue, enter both of these commands in the terminal to setup both the coffea environment and lpcjobqueue.

```
curl -OL https://raw.githubusercontent.com/CoffeaTeam/lpcjobqueue/main/bootstrap.sh
bash bootstrap.sh
```

If you've already done the above, or you have just run the above commands for the first time, you can run the executable as shown below to start the environment.

```
./shell
```

The `./shell` will get you into a singularity container with the required environment.  From within the container, Open a jupyter notebook with the command below, and you're good to go :)

```
jupyter notebook --ip 0.0.0.0 --no-browser
```

## Execute notebook

Go to [localhost](http://127.0.0.1:8888) to open the jupyter interface. 

## Get the exercises

Open the terminal via "New -> Terminal"

Then

```
git clone https://github.com/7quantumphysics/CoffeaJERC.git
```

The example notebook is [L2L3_profiles_demo.ipynb](https://github.com/7quantumphysics/CoffeaJERC/blob/master/L2L3_profiles_demo.ipynb).
