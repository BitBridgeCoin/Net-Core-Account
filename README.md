# Net-Core-Account
configurable Authentication&amp;Authorization Management

Below are principles and best practice to follow:    
(1) Authentication, authorization and Business Logic should be well separated.    
(2) Authorization is the process of verifying access permissions(employee,or another API) to resource     
(3) Authorization is hard to standardize and more of application specific. It’s better to implement it on official and popular framework and packages.[1]     
(4) Permission is the authorization rules with claims as parameters    
(5) Generally, every restricted resource has an access policy    
(6) Resources(section of code, edit or delete button, and etc),organization, permission provide different perspectives toauthorization system. Those concepts are not orthogonal.   
(7) Every protected resource should have an authorization(with policy name)   
(8) Policy name on resource should contain the organization meaning to reflect resource is expected to belongs to   
(9) We can group resources sharing the same policy authorization into to resource group   
(10) The resource owner has edit right   
(11) People of the higher rank in the hierarchy tree inherit the permissions   
(12) Exceptions are made into exception tables    
(13) ALL should be configurable    
