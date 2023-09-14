# SyntesisProject

#### requirements:
z3 solver- can be installed by running the command: **pip install z3-solver** in the terminal

tkinter python library for GUI  by running the command: **pip install tk** in the terminal
#### Project description:

#### Usage:

<img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/657e412d-494f-447d-a406-04f2294e185c">

#### Language specifications:
##### features:
* the project supports an expanded hoare language that contains:
     * Integer Holes - the project supports a sketch like hole system for Integers (inserted to the code as ??) and of strings (inserted to the code as ???).
                       the project will find a fill to the holes by using CEGIS method of synthesis and with asserts inserted by a user.
     * Asserts - a user can insert assertion to the code that restrict the program to follow certain conditions.
                
     * Strings - the project supports the inclusion of strings, a string constant value should be of the form: '<value>' , the program supports conctation of strings via                     the operator + and can find hole that contains a string value and will be inserted as ??? in the program.
                 String supports the @ operator too , for (a @ 2) the operator will return the character at index 2 from string a.
                 example:
       
<img width="958" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/9d942208-81f8-44ce-8e47-4e1b4a7c3163">

       
     * Boolean logical operations (add, or, not, ->) - used mostly for more difficult constraints in the conditions in while loop and asserts, in those condition the user can enter the logical keywords true , false if needed.
  
     * Arrays - the program supports array by a limited capacity. 
                array can be declared by the [<value1>,<value2>...] or [] or [<value1>], the values has to be numerical                      values or numerical value hole and each empty aray                   will be initialized to be zero array.
                Arrays supports the followind functions:
                * store - the function stores a value y in array cell x : a:= a store 1 1 for example will store the value 1                           in index 1 of the array a
                * select - the function gets the value at index x of the array : b:= a select 2 for example will return the                             value of the array in index 2

                example:
<img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/3b0da209-e9ad-49dc-9279-a628a748bd82">


     * For loops - the for loop is a simple multiplication function, it gets an integer n value (not a hole) and multiplies the code inside its do caluse n times
       
     * Modified arithmetic operations such as pow and mod - the project supports more arithmetic operation in order to give  maximal experience,
                                                            **for the pow operation the exponent cannot be a hole and has to be an integer or a value that has no dependency on holes**, the power operation allows to implement polynoms easily.
       example:
       <img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/03261260-518e-4e64-a7a9-3a77fd015fd0">
                                                
      
##### Inputs and outputs:
* In order to use the program you have to insert the designated example count, and unwinding size for  while loops in the program.
the proggram has unrolling feature for handeling while loops for the user content, and the program can handle as many examples as inserted.
* after filling those entries press the "create text button" in order to create text boxes for your PBE.
* an empty entry is an entry without examples, the example values should be given by the form of:
   <variable name> = <variable value>
                  or
  <variable name> = <variable value> ; <variable2 name> = <variable2 value> ....

in the PBE the types of vairables should be consistent
and array/string variables should be declared by an input to at least one empty example 
<img width="960" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/c3b1ba25-247c-455c-859e-410122dcc2e0">

false example, the Q condition does not apply -> the program will return a counter example:
<img width="959" alt="image" src="https://github.com/shalev5252/syntesisProject/assets/74376280/beb38d59-b5bb-4a6c-81ee-cfaf6b284608">
##### features


#### Open the app:
the aplication ui service is in the file syntApp.py. running it in the cmd line will open the project by using the command:
python syntApp.py


#### User Experience flow:

![user experience flow](https://github.com/shalev5252/syntesisProject/assets/74376280/b7a220a9-7661-4005-b01f-f7ca8e9a8d13)

#### Project calculation flow:
![calc_flow](https://github.com/shalev5252/syntesisProject/assets/74376280/1128fc8c-95b4-48cd-941b-e2c7e67e98e6)
