https://swagger.io/docs/specification/v2_0/what-is-swagger/


- Swagger allows you to describe the structure of your APIs so that machines can read them. The ability of APIs to describe their own structure is the root of all awesomeness in Swagger. Why is it so great? Well, by reading your API’s structure, we can automatically build beautiful and interactive API documentation. We can also automatically generate client libraries for your API in many languages and explore other possibilities like automated testing. Swagger does this by asking your API to return a YAML or JSON that contains a detailed description of your entire API. This file is essentially a resource listing of your API which adheres to OpenAPI Specification. The specification asks you to include information like:

What are all the operations that your API supports?
What are your API’s parameters and what does it return?
Does your API need some authorization?
And even fun things like terms, contact information and license to use the API.
You can write a Swagger spec for your API manually, or have it generated automatically from annotations in your source code. Check swagger.io/open-source-integrations for a list of tools that let you generate Swagger from code.
