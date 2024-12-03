# Lab3 Bufbomb
For this lab we had to analyze a vulnerable peice of code provided and find buffer overflow strings that would execute the necessary exploits. The method of exploitation was different for each of the three phases smoke, fizz, and bang. The description of each is below:
- Smoke: For smoke I just had to rewrite the return address on the stack to the address of the smoke function. The exploit string is in the smoke.txt file
- Fizz: For the fizz phase I had to rewrite the return address to the start of the fizz function and also put the value of my cookie (Generated from my student ID) at the top of the stack so the function could use it. The exploit string is in the fizz.txt file
- Bang: Finally, for bang I needed to write some assembly to the stack that would change the value of a global variable and then return to the bang function, which compares the global variable to my cookie value. The exploit string is in the bang.txt file.
