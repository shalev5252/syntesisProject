# SyntesisProject

#### Project description:

#### Usage:

<img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/657e412d-494f-447d-a406-04f2294e185c">


#### Language specifications:
* the project supports an expanded whore language that contains:
     * Strings - the project supports the inclusion of strings, a string constant value should be of the form: '<value>' , the program supports conctation of strings via                     the operator + and can find hole that contains a string value and will be inserted as ??? in the program.
                 String supports the @ operator too , for (a @ 2) the operator will return the character at index 2 from string a.
                 example:
<img width="958" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/9d942208-81f8-44ce-8e47-4e1b4a7c3163">

       
     * Boolean logical operations (add, or, not) - used mostly for more difficult constraints in the conditions in while loop and asserts.
  
     * Arrays - the program supports array by a limited capacity. **All the arrays in the program are of fixed size, 50 elements**,
                array can be declared by the [<value1>,<value2>...] or [] or [<value1>], the values has to be numerical values or numerical value hole and each empty aray                   will be initialized to be zero array.
                Arrays supports the followind functions:
                * store - the function stores a value y in array cell x : a:= a store 1 1 for example will store the value 1 in index 1 of the array a
                * select - the function gets the value at index x of the array : b:= a select 2 for example will return the value of the array in index 2
                           **since ArrayRef and Arrays in z3 are maps from index to value and they are infinite for all integer numbers there is no guarntee for the values                               the function will return for numbers that are larger than 49 and smaller than 0**
                * equals - the function will return boolean value if the arrays have the exact same mapping (for indexes 0-49)
                example:
<img width="948" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/590c1ddc-28d8-4a3f-89ab-5410866b600f">

     * For loops - the for loop is a simple multiplication function, it gets an integer n value (not a hole) and multiplies the code inside its do caluse n times
       
     * Modified arithmetic operations such as pow and mod - the project supports more arithmetic operation in order to give  maximal experience,
                                                            **for the pow operation the exponent cannot be a hole and has to be integer**, the power operation allows to implement polynoms easily.
       example:
       <img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/03261260-518e-4e64-a7a9-3a77fd015fd0">
                                                
      
#### Inputs and outputs:
* In order to use the program you have to insert the designated example count, and unwinding size for  while loops in the program.
the proggram has unrolling feature fir handeling while loops for the user content, and the program can handle as many examples as inserted.
* after filling those entries press the "create text button" in order to create text boxes for your pbe.
* an empty entry is an entry without examples, the example values shoul be given by the form of:
   <variable name> = <variable value>
                  or
  <variable name> = <variable value> ; <variable2 name> = <variable2 value> ....

in the PBE the types of vairables should be consistent
and array/string variables should be declared by an input to at least one empty example 
<img width="950" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/976275e2-7ddb-4a4f-8ec5-ce0606109c91">
<img width="954" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/ddfcbe4a-c122-45b7-b09d-b2ae9ddbae24">

#### Code examples:


