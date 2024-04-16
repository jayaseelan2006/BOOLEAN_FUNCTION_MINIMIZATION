# BOOLEAN_FUNCTION_MINIMIZATION
# Developed by:JAYASEELAN U
# RegisterNumber:212223220039
# AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

# Equipment Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Theory**



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);

input a,b,c,d,w,x,y,z;

output f1,f2;

wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;

not(adash,a);

not(bdash,b);

not(cdash,c);

not(ddash,d);

not(ydash,y);

and(p,bdash,ddash);

and(q,adash,b,d);

and(r,a,b,cdash);

or(f1,p,q,r);

//type code for f2 as like f1 endmodule

# Truth Table:
![222](https://github.com/jayaseelan2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/151389443/9d9891ce-3f23-4923-ab18-cbece04839a5)

![11](https://github.com/jayaseelan2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/151389443/b5bd1369-6822-4cfc-8a33-3b98f766ccd5)



# RTL realization:
![R](https://github.com/jayaseelan2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/151389443/4e4c70c5-b02e-486b-8490-73cc72e3c23d)


**Logic Diagram**
# Output:
![diagram](https://github.com/jayaseelan2006/BOOLEAN_FUNCTION_MINIMIZATION/assets/151389443/0bc3999d-98c1-42a6-99f4-8acd5c248fa7)




# Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

