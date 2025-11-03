# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:

![Image 2025-11-03 at 22 26 46_14619ee1](https://github.com/user-attachments/assets/adca2099-b187-45b8-b604-003da22aa4d5)
![Image 2025-11-03 at 22 26 46_ff1dda57](https://github.com/user-attachments/assets/9c7ffef4-89e6-4f73-8d34-251e3e1d20ec)
![Image 2025-11-03 at 22 26 45_11f185c7](https://github.com/user-attachments/assets/0271ff95-1f8f-4293-9116-23562d95be71)

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 

	num=[1];
	den=[1 15 50 0];
	sys=tf(num,den);
	rlocus(sys);
	[k,poles]=rlocfind(sys)

## Output: 

<img width="1916" height="1195" alt="image" src="https://github.com/user-attachments/assets/640c8a3c-6afb-416e-ab4b-4deaa55f0ec0" />

	Select a point in the graphics window
	
	selected_point =
	
	   0.0136 + 7.1062i
	
	
	k =
	
	  758.8391
	
	
	poles =
	
	 -15.0320 + 0.0000i
	   0.0160 + 7.1050i
	   0.0160 - 7.1050i

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is ------------
