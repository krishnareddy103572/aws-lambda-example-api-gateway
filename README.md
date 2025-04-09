# aws-lambda-example-api-gateway


1.Create a Backend Project with help of Code Editors like IntelliJ IDEA
  like create project with 
      1.a)catalog:Maven Central
      1.b)Archetype:com.amazonaws.serverless.archetypes:aws-serverless-springboot3-archetype(it ensures aws dependencies)



 2.After writing entity,controllers,service,repository all layers 
    2.a) run maven package to generate zip or jar (to host our application in aws lambda)

 3.Open AWS Lambda 
   3.a) create a function with name
   3.b)keep java as code 
   3.c) upload the zip into it

 4.Open AWS API GATEWAY
   4.a)click on create api
   4.b)use rest api
   4.c)give name to api
   4.d)click on create resource
   4.e)under resource name give this {proxy +} -> it is available in template.yml file in your project
   4.f)give method type = ANY
   4.g)in lambda function :we will find our lambada function then add it like this example(arn:aws:lambda:eu-west-1:3586078XXXXXX:function:YOUR LAMBDA         FUNCTION NAME and click on create method
   4.h)click on deploy api by giving name and stage as new stage 
   4.i)then you we will get like this https://pkgkghj5.....amazonaws.com/your stage name


   5.now you can add it into postman and make requests
   
   
   

      
