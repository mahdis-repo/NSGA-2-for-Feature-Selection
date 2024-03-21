# Multiple Objective Optimization Using NSGA-2 Algorithm

There are three methods of feature selection: Filter methods, Wrapper methods and Embedded methods.
This is a wrapper method in which selected features are being evaluated by a KNN (neighbors = 5). 

## NSGA-2 and binary desicion variables

We either select the feature (1) or we dont (1):


![image](https://github.com/mahdis-repo/NSGA-2-for-Feature-Selection/assets/145799768/dd6b0de1-27b4-4739-b56f-e68992bb37a9)

after getting the embeddings we have 80 features and here is the initial population:


![image](https://github.com/mahdis-repo/NSGA-2-for-Feature-Selection/assets/145799768/369262a0-e957-49e9-8b3c-a7461d98cdc6)


Objectives:

- error : 1 - accuracy
- number of features

  and we want to minimize both of our objective, after generating 100 populations of size 100:

  
  ![image](https://github.com/mahdis-repo/NSGA-2-for-Feature-Selection/assets/145799768/ef7e8def-b3e0-4ec9-a011-c6e5bbf3cb34)

  and that's pretty cool! we can classify embeddings with an accuracy of 97% using only 5 features!


### Installing

You may have Keras, Tensorflow and Scikit-Learn but you may need to install Pymoo. A multi-Objective Optimzation Library.
```
!pip install pymoo
```
<!--
## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds
-->
## Contributing

Contributions are always welcomed!

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

