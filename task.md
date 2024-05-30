* web
    * ingress
        * http (80): allow to all
        * ssh (22) : allow to all
* app
    * ingress
        * ssh (22) : allow to all
        * http (8080) : allow within the vpc range 
*  db
    * ingress 
        * tcp (3306) : allow within the vpc range 

Remove default values from inputs.tf as any new user must enter the attributes when using dev.tfvars file default values...so we remove default values from inputs.tf 