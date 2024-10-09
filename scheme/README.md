# How to run scheme

(Thanks to ProfessorHarveysNumberOneFan, see May 5, 2022 comment [here](https://archive.org/details/ucberkeley_webcast_l28HAzKy0N8).)

1. ```mkdir scheme```
2. ```cd scheme && touch simplyscm```
3. Copy the code from [here](https://people.eecs.berkeley.edu/~bh/ssch27/appendix-simply.html) into the file created in the previous step.
4. Install docker.
5. ```sudo docker pull stklos/stklos:latest```
6. ```sudo docker run -v $(pwd):/home -it stklos/stklos:latest```
7. ```stklos> (load "simplyscm")```

In case you are wondering how to get out of the container you run: ```,quit```.

Repeat steps 5 to 7 as needed.

Run ```docker container prune``` once in a while just to get rid of those accumulating stopped containers.

