The realization of the experiment

1. The execution order of angular application
    i. app.config()
    ii. then, app.run()
    iii. then, the controllers
    iv. but if the controllers are dependend upon services then they should be executed

2. The services are executed only once to create the service object, though some property 
    of the object is random variable

3. The controllers who use those services will get the same value of service unless one of those controllers change 
    the value of the services (by some getter/setter/custom method)

4. The config and the run method are also executed once for the lifetime of the angular 
    application

5. if some controller is not required it will not be executed ever.

6. When we change the view, then the controller of that route view gets executed.
