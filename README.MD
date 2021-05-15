DataEngineering HW #1 

A NIFI pipeline with Jupiter minimal notebook using docker-compose
It reads a csv file and transform it to a json file

The pipeline structure is as follows:
(Read the csv) >> (splits every record and transform it into a json record) >>
(merge json records into one json file) >> (rename json file) >> (save to the nifi running Docker container and the mounted volume on local disk)

The following YouTube video is a demo of running the implementation using the provided template (assiQ1_csvTOjson.xml):    

https://youtu.be/jjLd0n7sScA

the PPT has screenshots of the full creation process of the pipeline.

The following are abbreviated steps for deploying the pipeline, a full detailed demonstration can be found in the YouTube video (~11 min) or the PPT:
1.	Clone the repo.
2.	In the directory run ‘docker-compose up’
3.	Once all containers are up, please use:
-localhost:8887 to access Jupiter notebook 
-localhost:8087 to access NIFI
4. using the GUI, import the provided assiQ1_csvTOjson.xml templet.
5. activate all services
6. run the pipeline
7. the pipeline comes with a csv data file (data.csv), using the Jupiter notebook it is possible to create further data.


*Note: Docker is provided in the utilities*
*Note: you may need to navigate to where directory input/ is and run the chmod command,,,  ~$ chmod 777 input *

oRefai       
