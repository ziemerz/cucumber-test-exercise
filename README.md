# cucumber-test-exercise

I can see the use for Cucumber in business cases where you have non-technical people 
reading and writing tests. 

Cucumber makes it easy to translate Gherkin to tests. 
Where it would give the most value in the Gutenberg project would be for either unit tests, 
where we test actual business logic and for frontend testing, 
where we expect something to show on screen.

 
In the scenario of our Gutenberg project, 
where we don’t have any business logic in the application, other than in the queries we
make to our databases, we see a very limited potential for getting any value out of Cucumber. 
 
Also, we’re not communicating our tests to non-technical people in this project, which deprives even more value. 


For the case of profiling, we are definitely going to use a tool for this for our project. 
We're just not going to use JMeter as we don't want to be dependent on a GUI to generate our
configuration. 

Anyway, profiling is definitely something that adds value for us, as we're going to do benchmarks
between the various database technologies. Also, we're planning to test whether a de-normalized or
normalized PostgreSQL database will be fastest. 

When we're using profiling for our application, we're most likely measuring Spring Boots performance
rather than our codes performance. The only "logic" we're going to have, is we're going to 
implement a mapper so we can return a uniform object through our API.

I couldn't find a decent tool for generating test pairs for pairwise testing for Mac. Also, 
we probably wont need this for the Gutenberg project, as we don't have any boundaries or pairs
of data send to our API. We're only going to send single values.  