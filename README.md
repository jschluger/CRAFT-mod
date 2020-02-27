# CRAFT-mod

## Working with Submodules
This repository uses git submodules to refer to the CRAFT-backend and CRAFT-fronent repositories. Here are the basics of working with submodules in git. Consult [the documentation](https://git-scm.com/book/en/v2/Git-Tools-Submodules) for more details. 

### Cloning
*Step 1*: Run `$ git clone https://github.com/jschluger/CRAFT-mod.git tmp`

Now, CRAFT-backend and CRAFT-frontend are empty directories, not tracked as submodules.

*Step 2*: Run `$ git submodule init`

in order to initialize your local configuration file, ".gitmodules". CRAFT-backend and CRAFT-frontend are still empty directories.

*Step 3*: Run `$ git submodule update` 

in order to download the CRAFT-backend and CRAFT-frontend reposetories into their respective directories. You now have all the required code for the project!

## Running the Application
Once have cloned, initalized, and downloaded submodules, you are ready to run the project with docker.

*Step 1*: Run `$ docker-compose build` to build required images.

*Step 2*: Run `$ docker-compose up` to start running the two servers. 



#### Refrences
https://git-scm.com/book/en/v2/Git-Tools-Submodules
https://docs.docker.com/compose/
